# Tink (tink-com)

Tink, a Visa solution acquired in 2022, is a European Open Banking platform with 6,000+ bank connections across Europe and a US Pay by Bank stack. A single PSD2-licensed API exposes aggregated bank data (Accounts, Transactions, Balances, Identities, Investments, Loans), value-added risk reports (Account Check, Business Account Check, Income Check, Expense Check, Risk Insights, Risk Categorisation), Money Manager BFM, Data Enrichment, PSD2 Payment Initiation Services (Pay by Bank, Auto Payments, Variable Recurring Payments, Mandates, Refunds, Payouts), and a Connector API for pushing partner data into the platform. Authentication is OAuth 2.0 with delegated user consent handled by the Tink Link hosted flow.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - Open Banking, PSD2, Payment Initiation, Account Aggregation, Risk Decisioning, Pay by Bank, Finance, Banking, Europe, Visa

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Base URLs

| Region | URL |
|---|---|
| Tink EU Production | `https://api.tink.com` |
| Tink US Production | `https://api.us.tink.com` |

## APIs

### Tink OAuth API
OAuth 2.0 client-credentials, refresh, and delegated authorization-grant endpoints that gate every Tink API. Includes permanent user creation and Tink Link session delegation.

**Human URL:** [https://docs.tink.com/api-reference/auth-api](https://docs.tink.com/api-reference/auth-api)

- [Documentation](https://docs.tink.com/api-reference/auth-api)
- [OpenAPI](openapi/tink-oauth-api-openapi.yml)
- [Naftiko Capability — OAuth](capabilities/oauth.yaml)

### Tink Account Check API
Verify that a bank account belongs to the consumer or business presenting it. Returns verified account, identity, balance, and user-match results as JSON or PDF.

**Human URL:** [https://docs.tink.com/resources/account-check](https://docs.tink.com/resources/account-check)

- [Documentation](https://docs.tink.com/resources/account-check)
- [OpenAPI](openapi/tink-account-check-api-openapi.yml)
- [JSON Schema — Account Verification Report](json-schema/tink-account-verification-report-schema.json)
- [Example — Account Verification Report](examples/tink-account-verification-report-example.json)
- [Naftiko Capability — Account Check](capabilities/account-check.yaml)

### Tink Data API
Read consented bank data from 6,000+ European banks. Accounts, balances, transactions, account parties, identities, investment holdings, loan accounts, on-demand balance refresh, and credentials/consent management.

**Human URL:** [https://docs.tink.com/resources/transactions](https://docs.tink.com/resources/transactions)

- [Documentation](https://docs.tink.com/resources/transactions)
- [OpenAPI](openapi/tink-data-api-openapi.yml)
- [JSON Schema — Transaction](json-schema/tink-transaction-schema.json)
- [Example — Transaction](examples/tink-transaction-example.json)
- [Naftiko Capability — Data Transactions](capabilities/data-transactions.yaml)

### Tink Data Enrichment API
Categorise raw bank transactions, identify the merchant, detect confirmed recurring transactions, and predict future recurring payments.

**Human URL:** [https://docs.tink.com/resources/data-enrichment](https://docs.tink.com/resources/data-enrichment)

- [Documentation](https://docs.tink.com/resources/data-enrichment)
- [OpenAPI](openapi/tink-data-enrichment-api-openapi.yml)
- [Naftiko Capability — Data Enrichment](capabilities/data-enrichment.yaml)

### Tink Payments API
PSD2 Payment Initiation Services. Initiate single payments, refunds, payouts, and create mandates for Auto Payments and sweeping Variable Recurring Payments. Available in EU and US.

**Human URL:** [https://docs.tink.com/resources/payments](https://docs.tink.com/resources/payments)

- [Documentation](https://docs.tink.com/resources/payments)
- [OpenAPI](openapi/tink-payments-api-openapi.yml)
- [JSON Schema — Payment](json-schema/tink-payment-schema.json)
- [Example — Payment](examples/tink-payment-example.json)
- [Naftiko Capability — Payments](capabilities/payments.yaml)

### Tink Risk and Reports API
Decisioning-grade reports built on aggregated bank data: Income Check, Expense Check, Risk Insights, and Risk Categorisation.

**Human URL:** [https://docs.tink.com/resources/risk-insights](https://docs.tink.com/resources/risk-insights)

- [Documentation — Risk Insights](https://docs.tink.com/resources/risk-insights)
- [Documentation — Income Check](https://docs.tink.com/resources/income-check)
- [Documentation — Expense Check](https://docs.tink.com/resources/expense-check)
- [OpenAPI](openapi/tink-risk-reports-api-openapi.yml)
- [Naftiko Capability — Risk and Reports](capabilities/risk-reports.yaml)

### Tink Money Manager API
Personal and business financial-management surface. Cash-flow summaries, budgets, financial calendar, and reconciliations.

**Human URL:** [https://docs.tink.com/resources/money-manager](https://docs.tink.com/resources/money-manager)

- [Documentation](https://docs.tink.com/resources/money-manager)
- [OpenAPI](openapi/tink-money-manager-api-openapi.yml)
- [Naftiko Capability — Money Manager](capabilities/money-manager.yaml)

### Tink Connector API
Push partner-collected accounts and transactions into the Tink platform so they benefit from categorisation, recurring detection, Money Manager, and risk reporting.

**Human URL:** [https://docs.tink.com/resources/connector](https://docs.tink.com/resources/connector)

- [Documentation](https://docs.tink.com/resources/connector)
- [OpenAPI](openapi/tink-connector-api-openapi.yml)
- [Naftiko Capability — Connector](capabilities/connector.yaml)

### Tink Webhooks API
Asynchronous event notifications when reports complete, payments and refunds change status, or consented bank data refreshes.

**Human URL:** [https://docs.tink.com/resources/webhooks](https://docs.tink.com/resources/webhooks)

- [Documentation](https://docs.tink.com/resources/webhooks)
- [OpenAPI](openapi/tink-webhooks-api-openapi.yml)
- [Naftiko Capability — Webhooks](capabilities/webhooks.yaml)

## Common Properties

- [Portal](https://tink.com/)
- [Developer Docs](https://docs.tink.com/)
- [Console](https://console.tink.com/)
- [Contact Sales](https://tink.com/contact-sales/)
- [Pricing](https://tink.com/pricing/)
- [Status](https://status.tink.com/)
- [Changelog](https://docs.tink.com/changelog)
- [Blog](https://tink.com/blog/)
- [Terms of Service](https://tink.com/terms-and-conditions/)
- [Privacy Policy](https://tink.com/privacy-policy/)
- [Security](https://tink.com/security/)
- [GitHub Organization](https://github.com/tink-ab)
- [LinkedIn](https://www.linkedin.com/company/tink-ab/)
- [Postman Collections (EU)](https://github.com/tink-ab/tink-postman)
- [Postman Collections (US)](https://github.com/tink-ab/tink-postman-us)
- [SDK — Tink Link Android](https://github.com/tink-ab/tink-link-android)
- [SDK — Tink Link iOS](https://github.com/tink-ab/tink-link-ios)
- [SDK — Money Manager Android](https://github.com/tink-ab/tink-money-manager-android)
- [SDK — Money Manager iOS](https://github.com/tink-ab/tink-money-manager-ios)
- [Spectral Ruleset](rules/tink-rules.yml)
- [Vocabulary](vocabulary/tink-com-vocabulary.yml)
- [JSON-LD Context](json-ld/tink-com-context.jsonld)
- [Plans and Pricing](plans/tink-com-plans-pricing.yml)
- [Rate Limits](rate-limits/tink-com-rate-limits.yml)
- [FinOps Surface](finops/tink-com-finops.yml)

## Features

- 6,000+ bank connections across Europe (Nordics, UK, DACH, Benelux, France, Iberia, Italy, Ireland, Poland).
- PSD2 Payment Initiation for one-off payments, VRPs, Auto Payments, payouts, refunds, and mandates.
- Account Check and Business Account Check with optional identity match (name, DOB, address).
- Risk Insights and Risk Categorisation reports for affordability and lending.
- Income Check and Expense Check for underwriting and KYC.
- Money Manager BFM: cash-flow, budgets, financial calendar, reconciliations.
- Data Enrichment: Tink categorisation, merchant identification, recurring detection and prediction.
- Connector API: push partner-collected accounts and transactions into Tink.
- Tink Link hosted consent UX with SCA and app-to-app redirects.
- Webhooks for asynchronous events.
- SOC 2 Type II and PSD2 licensed — customers do not need their own PSD2 authorisation.

## Use Cases

- Onboarding and KYC via verified account ownership.
- Affordability and underwriting using Risk Insights, Income Check, and Expense Check.
- Pay by Bank checkout with one-off PIS or Auto Payments.
- Subscription billing with sweeping VRPs.
- Embedded BFM for SMB banking and accounting apps.
- PFM and personal-banking categorisation.
- Payouts to verified bank accounts.
- Open Finance composition stitching PSD2 and partner data via Connector.

## Plans

Tink publishes two commercial tiers — **Standard** and **Enterprise** — with per-call pricing quoted privately to existing customers. Net-new prospects engage Tink sales for a quote.

| Tier | Products |
|---|---|
| Standard | Account Check, Transactions, Tink Link, on-demand refresh |
| Enterprise | Standard + Risk Insights, Income Check, Expense Check, Business Account Check, Business Transactions, Money Manager, Payment Initiation; background refresh; guaranteed SLAs |

Full machine-readable plans live in [plans/tink-com-plans-pricing.yml](plans/tink-com-plans-pricing.yml).

## Rate Limits

Specific RPS / RPM limits are not publicly disclosed; Tink configures them per-client per-product at contract signing. PSD2 imposes a four-per-24-hours background-refresh cap per consent without SCA. See [rate-limits/tink-com-rate-limits.yml](rate-limits/tink-com-rate-limits.yml).

## FinOps

FOCUS-aligned billing-surface definition lives in [finops/tink-com-finops.yml](finops/tink-com-finops.yml). Meters include account-check reports, business-account-check reports, income/expense/risk reports, PIS payments initiated and executed, refunds, active continuous-access users, and data-API requests.

## Integrations

Adyen, Revolut, Younited, Bank Norwegian, PostNord Strålfors, and the broader Visa risk and payments stack since the 2022 acquisition.
