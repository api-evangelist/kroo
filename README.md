# Kroo

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Kroo Bank Ltd is a UK app-based challenger bank, founded in 2016 and granted a full UK banking licence by the PRA/FCA in 2021 (restrictions lifted in 2022), that launched its digital-only personal current account in December 2022. Independent and venture-backed rather than mutual or part of a larger group, Kroo offers a fee-free everyday current account, interest-paying balances and "Kroo Pots", fee-free spending abroad, and FSCS deposit protection up to GBP 85,000. As an FCA-authorised ASPSP under PSD2, Kroo is a regulated Open Banking provider (though not one of the nine CMA9-mandated banks and, as a branchless digital bank, it publishes no Open Data reference APIs for ATMs or branches). It exposes the UK Open Banking Implementation Entity (OBIE) Read/Write API family - Account and Transaction Information, Payment Initiation, and Confirmation of Funds - through a Banfico-hosted developer portal at developer.kroo.banfico.io, secured with FAPI-grade OAuth2/OIDC, PSD2 strong customer authentication implemented as a CIBA decoupled (poll-mode) flow, and mutual-TLS client authentication using OBIE/eIDAS certificates, validated with the OpenID Foundation conformance suite.

**Areas:** Financial Services · Banking · Open Banking · PSD2 · OBIE · FAPI · United Kingdom · Payments · Account Information · Challenger Bank · Fintech

## Kroo on APIs.io

Everything profiled for Kroo is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/kroo/](https://apis.io/providers/kroo/)** — or go straight to one of the APIs or properties below.

### APIs (28)

- [Kroo Account Access Consents API](https://apis.io/apis/kroo/kroo-account-access-consents-api/) — The Account Access Consents API from Kroo — 2 operation(s) for account access consents.
- [Kroo Accounts API](https://apis.io/apis/kroo/kroo-accounts-api/) — The Accounts API from Kroo — 2 operation(s) for accounts.
- [Kroo Balances API](https://apis.io/apis/kroo/kroo-balances-api/) — The Balances API from Kroo — 2 operation(s) for balances.
- [Kroo Beneficiaries API](https://apis.io/apis/kroo/kroo-beneficiaries-api/) — The Beneficiaries API from Kroo — 2 operation(s) for beneficiaries.
- [Kroo Direct Debits API](https://apis.io/apis/kroo/kroo-direct-debits-api/) — The Direct Debits API from Kroo — 2 operation(s) for direct debits.
- [Kroo Domestic Payment Consents API](https://apis.io/apis/kroo/kroo-domestic-payment-consents-api/) — The Domestic Payment Consents API from Kroo — 3 operation(s) for domestic payment consents.
- [Kroo Domestic Payments API](https://apis.io/apis/kroo/kroo-domestic-payments-api/) — The Domestic Payments API from Kroo — 3 operation(s) for domestic payments.
- [Kroo Domestic Scheduled Payment Consents API](https://apis.io/apis/kroo/kroo-domestic-scheduled-payment-consents-api/) — The Domestic Scheduled Payment Consents API from Kroo — 2 operation(s) for domestic scheduled payment consents.
- [Kroo Domestic Scheduled Payments API](https://apis.io/apis/kroo/kroo-domestic-scheduled-payments-api/) — The Domestic Scheduled Payments API from Kroo — 3 operation(s) for domestic scheduled payments.
- [Kroo Domestic Standing Order Consents API](https://apis.io/apis/kroo/kroo-domestic-standing-order-consents-api/) — The Domestic Standing Order Consents API from Kroo — 2 operation(s) for domestic standing order consents.
- [Kroo Domestic Standing Orders API](https://apis.io/apis/kroo/kroo-domestic-standing-orders-api/) — The Domestic Standing Orders API from Kroo — 3 operation(s) for domestic standing orders.
- [Kroo File Payment Consents API](https://apis.io/apis/kroo/kroo-file-payment-consents-api/) — The File Payment Consents API from Kroo — 3 operation(s) for file payment consents.
- [Kroo File Payments API](https://apis.io/apis/kroo/kroo-file-payments-api/) — The File Payments API from Kroo — 4 operation(s) for file payments.
- [Kroo Funds Confirmation Consents API](https://apis.io/apis/kroo/kroo-funds-confirmation-consents-api/) — The Funds Confirmation Consents API from Kroo — 2 operation(s) for funds confirmation consents.
- [Kroo Funds Confirmations API](https://apis.io/apis/kroo/kroo-funds-confirmations-api/) — The Funds Confirmations API from Kroo — 1 operation(s) for funds confirmations.
- [Kroo International Payment Consents API](https://apis.io/apis/kroo/kroo-international-payment-consents-api/) — The International Payment Consents API from Kroo — 3 operation(s) for international payment consents.
- [Kroo International Payments API](https://apis.io/apis/kroo/kroo-international-payments-api/) — The International Payments API from Kroo — 3 operation(s) for international payments.
- [Kroo International Scheduled Payments API](https://apis.io/apis/kroo/kroo-international-scheduled-payments-api/) — The International Scheduled Payments API from Kroo — 3 operation(s) for international scheduled payments.
- [Kroo International Scheduled Payments Consents API](https://apis.io/apis/kroo/kroo-international-scheduled-payments-consents-api/) — The International Scheduled Payments Consents API from Kroo — 3 operation(s) for international scheduled payments consents.
- [Kroo International Standing Orders API](https://apis.io/apis/kroo/kroo-international-standing-orders-api/) — The International Standing Orders API from Kroo — 3 operation(s) for international standing orders.
- [Kroo International Standing Orders Consents API](https://apis.io/apis/kroo/kroo-international-standing-orders-consents-api/) — The International Standing Orders Consents API from Kroo — 2 operation(s) for international standing orders consents.
- [Kroo Offers API](https://apis.io/apis/kroo/kroo-offers-api/) — The Offers API from Kroo — 2 operation(s) for offers.
- [Kroo Parties API](https://apis.io/apis/kroo/kroo-parties-api/) — The Parties API from Kroo — 3 operation(s) for parties.
- [Kroo Products API](https://apis.io/apis/kroo/kroo-products-api/) — The Products API from Kroo — 2 operation(s) for products.
- [Kroo Scheduled Payments API](https://apis.io/apis/kroo/kroo-scheduled-payments-api/) — The Scheduled Payments API from Kroo — 2 operation(s) for scheduled payments.
- [Kroo Standing Orders API](https://apis.io/apis/kroo/kroo-standing-orders-api/) — The Standing Orders API from Kroo — 2 operation(s) for standing orders.
- [Kroo Statements API](https://apis.io/apis/kroo/kroo-statements-api/) — The Statements API from Kroo — 5 operation(s) for statements.
- [Kroo Transactions API](https://apis.io/apis/kroo/kroo-transactions-api/) — The Transactions API from Kroo — 2 operation(s) for transactions.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [kroo](https://apis.io/servers/kroo/kroo/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Kroo Agentic Access](https://apis.io/agentic-access/kroo/kroo-agentic-access/)

#### Overlays (3)

OpenAPI overlays, including conversational phrasing for each operation.

- [Kroo Account Info Overlay](https://apis.io/overlays/kroo/kroo-account-info-overlay/)
- [Kroo Confirmation Funds Overlay](https://apis.io/overlays/kroo/kroo-confirmation-funds-overlay/)
- [Kroo Payment Initiation Overlay](https://apis.io/overlays/kroo/kroo-payment-initiation-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Kroo Authentication](https://apis.io/security/kroo/kroo-authentication/)
- [Kroo Domain Security](https://apis.io/security/kroo/kroo-domain-security/)
- [Kroo Vulnerability Disclosure](https://apis.io/security/kroo/kroo-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Kroo Scopes](https://apis.io/scopes/kroo/kroo-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.kroo.com/)
- [Documentation](https://kroo.com/open-banking-performance)
- [Support](https://www.kroo.com/support-is-here)
- [Blog](https://www.kroo.com/blog)
- [Security](https://kroo.com/.well-known/security.txt)
- [Terms of service](https://www.kroo.com/terms-of-use)
- [Privacy policy](https://www.kroo.com/privacy-notices)
- [Status](https://status.kroo.com/)

## API Evangelist rating

**Kin Score 37.5** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 69.6 |
| Contract quality | 49.0 |
| Contract governance | 4.5 |
| Operational transparency | 26.3 |
| Developer ergonomics | 37.5 |
| Access clarity | 21.1 |

**Agent readiness 35.4** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | negotiable (partial credit) |
| Idempotency | verified |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | verified |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | documented (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 42.5** — Banking & Open Finance

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/kroo/](https://apis.io/providers/kroo/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Kroo: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/kroo/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
