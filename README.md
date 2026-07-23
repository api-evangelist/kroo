# Kroo (kroo)

Kroo Bank Ltd is a UK app-based challenger bank, granted a full UK banking licence in 2021 and launching its digital-only personal current account in December 2022. As an FCA-authorised ASPSP under PSD2, Kroo is a regulated UK Open Banking provider (though not one of the CMA9-mandated banks, and as a branchless digital bank it publishes no Open Data reference APIs). It exposes the OBIE Read/Write API family through a Banfico-hosted developer portal, secured with FAPI-grade OAuth2/OIDC, mutual-TLS, and PSD2 strong customer authentication implemented as a CIBA decoupled flow.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/kroo/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/kroo/refs/heads/main/apis.yml)

## Tags

- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
- Challenger Bank
- Fintech

## Timestamps

- **Created:** 2026-07-23
- **Modified:** 2026-07-23

## APIs

### Kroo Account and Transaction Information API

Kroo's PSD2 Account Information Service (AIS) dedicated interface, conformant to the OBIE Read/Write Account and Transaction API Standard. Lets FCA-authorised AISP third parties retrieve, with customer consent, account details, balances, transactions, beneficiaries, standing orders, direct debits, scheduled payments, and statements. FAPI-secured (OAuth2/OIDC + mTLS + PSD2 SCA via CIBA); access requires TPP onboarding through the Kroo developer portal.

- **Human URL:** [https://developer.kroo.banfico.io/](https://developer.kroo.banfico.io/)

#### Tags

- Account Information
- AIS
- Open Banking
- OBIE

#### Properties

- [OpenAPI](openapi/obie-account-info-openapi.yaml) — OBIE Read/Write Account and Transaction API Standard v4.0.1 (shared standard, not a Kroo-proprietary contract)
- [Documentation](https://developer.kroo.banfico.io/)
- [API Reference](https://github.com/OpenBankingUK/read-write-api-specs)
- [Documentation](https://kroo.com/blog/open-banking-at-kroo)

### Kroo Payment Initiation API

Kroo's PSD2 Payment Initiation Service (PIS) dedicated interface, conformant to the OBIE Read/Write Payment Initiation API Standard. Lets FCA-authorised PISP third parties initiate domestic payments, scheduled payments, standing orders, and file payments from a customer's Kroo current account with their consent. FAPI-secured (OAuth2/OIDC + mTLS + PSD2 SCA via CIBA); access requires TPP onboarding through the Kroo developer portal.

- **Human URL:** [https://developer.kroo.banfico.io/](https://developer.kroo.banfico.io/)

#### Tags

- Payment Initiation
- PIS
- Open Banking
- OBIE

#### Properties

- [OpenAPI](openapi/obie-payment-initiation-openapi.yaml) — OBIE Read/Write Payment Initiation API Standard v4.0.1 (shared standard, not a Kroo-proprietary contract)
- [Documentation](https://developer.kroo.banfico.io/)
- [API Reference](https://github.com/OpenBankingUK/read-write-api-specs)
- [Documentation](https://kroo.com/blog/open-banking-at-kroo)

### Kroo Confirmation of Funds API

Kroo's PSD2 Confirmation of Funds Service (CBPII) dedicated interface, conformant to the OBIE Read/Write Confirmation of Funds API Standard. Lets FCA-authorised CBPII third parties confirm, with customer consent, whether a specified amount is available on a Kroo account without disclosing the balance. FAPI-secured (OAuth2/OIDC + mTLS + PSD2 SCA via CIBA); access requires TPP onboarding through the Kroo developer portal.

- **Human URL:** [https://developer.kroo.banfico.io/](https://developer.kroo.banfico.io/)

#### Tags

- Confirmation of Funds
- CBPII
- Open Banking
- OBIE

#### Properties

- [OpenAPI](openapi/obie-confirmation-funds-openapi.yaml) — OBIE Read/Write Confirmation of Funds API Standard v4.0.1 (shared standard, not a Kroo-proprietary contract)
- [Documentation](https://developer.kroo.banfico.io/)
- [API Reference](https://github.com/OpenBankingUK/read-write-api-specs)
- [Documentation](https://kroo.com/blog/open-banking-at-kroo)

## Common Properties

- [Website](https://www.kroo.com/)
- [Developer Portal](https://developer.kroo.banfico.io/)
- [Documentation](https://kroo.com/open-banking-performance)
- [Status Page](https://status.kroo.com/)
- [Blog](https://www.kroo.com/blog)
- [Support](https://www.kroo.com/support-is-here)
- [Terms of Service](https://www.kroo.com/terms-of-use)
- [Privacy Policy](https://www.kroo.com/privacy-notices)
- [LinkedIn](https://www.linkedin.com/company/kroobank)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
