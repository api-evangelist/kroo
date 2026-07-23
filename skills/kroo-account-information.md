---
name: Retrieve Kroo account data with an AIS consent
description: >-
  Obtain a PSU account-access consent and read accounts, balances, and
  transactions from Kroo's OBIE Account & Transaction Information API under
  FAPI-secured, consent-gated access.
api: openapi/obie-account-info-openapi.yaml
operations:
  - CreateAccountAccessConsents
  - GetAccountAccessConsentsConsentId
  - GetAccounts
  - GetAccountsAccountId
  - GetAccountsAccountIdBalances
  - GetAccountsAccountIdTransactions
---

# Retrieve Kroo account data (AIS)

Kroo is an FCA-authorised ASPSP. Access requires a registered AISP with OBIE/eIDAS
certificates onboarded through the Kroo (Banfico) developer portal. All calls use
mTLS, a FAPI `x-fapi-interaction-id` header, and a bearer access token.

## Steps

1. **Get a client-credentials token.** Authenticate as the TPP using
   `TPPOAuth2Security` (client_credentials, `accounts` scope), presenting the mTLS
   client certificate.
2. **Create the consent** — `CreateAccountAccessConsents`. POST an `OBReadConsent1`
   listing the permissions (e.g. `ReadAccountsDetail`, `ReadBalances`,
   `ReadTransactionsDetail`) and expiry. Capture the returned `ConsentId`.
3. **PSU authorisation / SCA.** Redirect (or CIBA decoupled poll via
   `PSUOAuth2Security`, authorization_code) so the customer approves the consent
   and Strong Customer Authentication completes. This yields a PSU access token.
4. **Confirm the consent** — `GetAccountAccessConsentsConsentId` to verify status
   is `Authorised`.
5. **List accounts** — `GetAccounts` with the PSU token.
6. **Read detail** — `GetAccountsAccountId`, `GetAccountsAccountIdBalances`,
   `GetAccountsAccountIdTransactions` for each `AccountId`.

## Rules

- Send `x-fapi-interaction-id` on every request and log the echoed value for tracing.
- Handle OBIE errors via the `OBErrorResponse1` envelope (see `errors/kroo-problem-types.yml`);
  a `401` with `UK.OBIE.Reauthenticate` means the PSU must re-authenticate.
- Respect `429` rate limits and the consent expiry; a revoked/expired consent returns `403`.
