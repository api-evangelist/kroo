---
name: Initiate a Kroo domestic payment (PIS)
description: >-
  Register a payment consent, obtain PSU authorisation, and initiate an
  idempotent domestic payment through Kroo's OBIE Payment Initiation API.
api: openapi/obie-payment-initiation-openapi.yaml
operations:
  - CreateDomesticPaymentConsents
  - GetDomesticPaymentConsentsConsentId
  - CreateDomesticPayments
  - GetDomesticPaymentsDomesticPaymentId
---

# Initiate a Kroo domestic payment (PIS)

Requires a registered PISP with OBIE/eIDAS certificates onboarded through the Kroo
(Banfico) developer portal. All calls use mTLS, FAPI headers, a detached JWS
signature, and PSD2 Strong Customer Authentication.

## Steps

1. **Get a client-credentials token** (`TPPOAuth2Security`, `payments` scope) over mTLS.
2. **Create the payment consent** — `CreateDomesticPaymentConsents`. POST an
   `OBWriteDomesticConsent4` with the debtor/creditor and `InstructedAmount`.
   Include the `x-jws-signature` header. Capture the `ConsentId`.
3. **PSU authorisation + SCA** via `PSUOAuth2Security` (authorization_code) or the
   CIBA decoupled poll flow, producing a PSU access token bound to the consent.
4. **Verify consent** — `GetDomesticPaymentConsentsConsentId` returns status
   `Authorised`.
5. **Initiate the payment** — `CreateDomesticPayments`. Send a **unique
   `x-idempotency-key`** (≤40 chars) so retries never double-pay; include the
   `x-jws-signature`. The `ConsentId` in the body must match the authorised consent.
6. **Poll status** — `GetDomesticPaymentsDomesticPaymentId` until the payment
   reaches a terminal status.

## Rules

- **Idempotency is mandatory on `CreateDomesticPayments`.** Reusing the same key
  with an identical body returns the original payment; a different body yields `409`.
- A `ConsentId` mismatch or business-rule failure surfaces as `422`
  (`UK.OBIE.Resource.ConsentMismatch` / `UK.OBIE.Rules.*`).
- Always send and log `x-fapi-interaction-id`; honour `429` back-off.
- See `conventions/kroo-conventions.yml` and `errors/kroo-problem-types.yml`.
