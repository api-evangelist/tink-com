# Tink (tink-com)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Tink, a Visa solution acquired in 2022, is a European Open Banking platform with 6,000+ bank connections across Europe and a US Pay by Bank stack. Tink exposes a single API for PSD2-aggregated bank data (Accounts, Transactions, Balances, Identities, Investments, Loans), value-added risk reports (Account Check, Business Account Check, Income Check, Expense Check, Risk Insights, Risk Categorisation), Money Manager BFM, Data Enrichment, and PSD2 Payment Initiation Services (Pay by Bank, Auto Payments, Variable Recurring Payments, Mandates, Refunds, Payouts). Authentication is OAuth 2.0 with delegated user consent through the Tink Link hosted flow.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/apis.yml)

## Scope

- **Access:** 3rd-Party

## Tags

- Open Banking
- PSD2
- Payment Initiation
- Account Aggregation
- Risk Decisioning
- Pay by Bank
- Finance
- Banking
- Europe
- Visa

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Tink OAuth API

OAuth 2.0 client-credentials, refresh, and delegated authorization-grant endpoints that gate every Tink API. Includes permanent user creation and Tink Link session delegation.

- **Human URL:** [https://docs.tink.com/api-reference/auth-api](https://docs.tink.com/api-reference/auth-api)
- **Base URL:** `https://api.tink.com`

#### Tags

- OAuth
- Authentication
- Users

#### Properties

- [Documentation](https://docs.tink.com/api-reference/auth-api)
- [OpenAPI](openapi/tink-oauth-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tink-oauth-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tink-oauth-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tink Account Check API

Verify that a bank account belongs to the consumer or business presenting it. Returns verified account, identity, balance, and user-match results as JSON or PDF. Includes Business Account Check and Tink Link session creation with user info for identity matching.

- **Human URL:** [https://docs.tink.com/resources/account-check](https://docs.tink.com/resources/account-check)
- **Base URL:** `https://api.tink.com`

#### Tags

- Account Check
- Account Verification
- KYC
- Onboarding

#### Properties

- [Documentation](https://docs.tink.com/resources/account-check)
- [OpenAPI](openapi/tink-account-check-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tink-account-check-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tink-account-check-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/tink-account-verification-report-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/tink-account-verification-report-example.json)

### Tink Data API

Read consented bank data from 6,000+ European banks. Lists accounts, balances, transactions, account parties, identities, investment holdings, and loan accounts. Includes on-demand balance refresh, credentials management, and provider-consent inspection.

- **Human URL:** [https://docs.tink.com/resources/transactions](https://docs.tink.com/resources/transactions)
- **Base URL:** `https://api.tink.com`

#### Tags

- Accounts
- Transactions
- Balances
- Identities
- Investments
- Loans

#### Properties

- [Documentation](https://docs.tink.com/resources/transactions)
- [OpenAPI](openapi/tink-data-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tink-data-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tink-data-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/tink-transaction-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/tink-transaction-example.json)

### Tink Data Enrichment API

Categorise raw bank transactions, identify the merchant, detect confirmed recurring transactions, and predict future recurring payments. Powers Money Manager, Expense Check, Income Check, and Risk Insights downstream.

- **Human URL:** [https://docs.tink.com/resources/data-enrichment](https://docs.tink.com/resources/data-enrichment)
- **Base URL:** `https://api.tink.com`

#### Tags

- Data Enrichment
- Categorisation
- Recurring Transactions
- Merchants

#### Properties

- [Documentation](https://docs.tink.com/resources/data-enrichment)
- [OpenAPI](openapi/tink-data-enrichment-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tink-data-enrichment-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tink-data-enrichment-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tink Payments API

PSD2 Payment Initiation Services. Initiate single payments, refunds, payouts, and create mandates for Auto Payments and sweeping Variable Recurring Payments. Available in EU under PSD2 and in the US via the Pay by Bank stack at api.us.tink.com.

- **Human URL:** [https://docs.tink.com/resources/payments](https://docs.tink.com/resources/payments)
- **Base URL:** `https://api.tink.com`

#### Tags

- Payments
- Payment Initiation
- PSD2
- Pay by Bank
- Mandates
- Refunds
- Variable Recurring Payments

#### Properties

- [Documentation](https://docs.tink.com/resources/payments)
- [OpenAPI](openapi/tink-payments-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tink-payments-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tink-payments-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/tink-payment-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/tink-payment-example.json)

### Tink Risk and Reports API

Decisioning-grade reports built on aggregated bank data — Income Check, Expense Check, Risk Insights, and Risk Categorisation — for affordability, underwriting, and lending decisions.

- **Human URL:** [https://docs.tink.com/resources/risk-insights](https://docs.tink.com/resources/risk-insights)
- **Base URL:** `https://api.tink.com`

#### Tags

- Risk
- Income Check
- Expense Check
- Risk Insights
- Risk Categorisation
- Lending
- Affordability

#### Properties

- [Documentation](https://docs.tink.com/resources/risk-insights)
- [Documentation](https://docs.tink.com/resources/income-check)
- [Documentation](https://docs.tink.com/resources/expense-check)
- [OpenAPI](openapi/tink-risk-reports-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tink-risk-reports-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tink-risk-reports-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tink Money Manager API

Personal and business financial-management surface. Cash-flow summaries, recurring and one-off business budgets, a financial calendar of bills and invoices, and reconciliations against bank transactions.

- **Human URL:** [https://docs.tink.com/resources/money-manager](https://docs.tink.com/resources/money-manager)
- **Base URL:** `https://api.tink.com`

#### Tags

- Money Manager
- BFM
- Cash Flow
- Budgets
- Financial Calendar

#### Properties

- [Documentation](https://docs.tink.com/resources/money-manager)
- [OpenAPI](openapi/tink-money-manager-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tink-money-manager-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tink-money-manager-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tink Connector API

Push partner-collected accounts and transactions into the Tink platform so they benefit from Tink categorisation, recurring detection, Money Manager, and risk reporting alongside PSD2-aggregated data.

- **Human URL:** [https://docs.tink.com/resources/connector](https://docs.tink.com/resources/connector)
- **Base URL:** `https://api.tink.com`

#### Tags

- Connector
- Data Ingestion

#### Properties

- [Documentation](https://docs.tink.com/resources/connector)
- [OpenAPI](openapi/tink-connector-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tink-connector-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tink-connector-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tink Webhooks API

Register webhook endpoints that receive asynchronous events when reports are ready, payments and refunds change status, or consented bank data is refreshed.

- **Human URL:** [https://docs.tink.com/resources/webhooks](https://docs.tink.com/resources/webhooks)
- **Base URL:** `https://api.tink.com`

#### Tags

- Webhooks
- Events

#### Properties

- [Documentation](https://docs.tink.com/resources/webhooks)
- [OpenAPI](openapi/tink-webhooks-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tink-webhooks-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tink-webhooks-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://tink.com/)
- [Documentation](https://docs.tink.com/)
- [Console](https://console.tink.com/)
- [Sign Up](https://tink.com/contact-sales/)
- [Pricing](https://tink.com/pricing/)
- [Status Page](https://status.tink.com/)
- [Changelog](https://docs.tink.com/changelog)
- [Blog](https://tink.com/blog/)
- [Terms of Service](https://tink.com/terms-and-conditions/)
- [Privacy Policy](https://tink.com/privacy-policy/)
- [Security](https://tink.com/security/)
- [GitHub Organization](https://github.com/tink-ab)
- [LinkedIn](https://www.linkedin.com/company/tink-ab/)
- [Postman](https://github.com/tink-ab/tink-postman) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Postman](https://github.com/tink-ab/tink-postman-us) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [SDK](https://github.com/tink-ab/tink-link-android)
- [SDK](https://github.com/tink-ab/tink-link-ios)
- [SDK](https://github.com/tink-ab/tink-money-manager-android)
- [SDK](https://github.com/tink-ab/tink-money-manager-ios)
- [Tools](https://github.com/tink-ab/terraform-provider-buildkite)
- [Spectral Rules](rules/tink-rules.yml)
- [Vocabulary](vocabulary/tink-com-vocabulary.yml)
- [JSON-LD](json-ld/tink-com-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Plans](plans/tink-com-plans-pricing.yml)
- [Rate Limits](rate-limits/tink-com-rate-limits.yml)
- [Fin Ops](finops/tink-com-finops.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** API Evangelist
**Email:** info@apievangelist.com
