# SmartSave

**SmartSave Beta 1.3.14 — Release Candidate / Beta Deployment**

SmartSave brings income and expense tracking, budgets, savings goals, CSV statement imports, and financial analysis into a private Telegram conversation. Guided entry and text-based input make everyday bookkeeping available without a separate dashboard.

> This is a documentation-only portfolio showcase of a private Python application. No runnable bot, production source, credentials, or financial records are included.

## What SmartSave does

| Area | Implemented capabilities |
| --- | --- |
| Track | Income and expenses, confirmation and editing, categories, history, statistics |
| Organize | Accounts, opening balances, reconciliation, linked transfers |
| Plan | Category budgets, progress, savings goals, forecasts |
| Import | CSV validation, preview, category review, confirmation, duplicate protection |
| Understand | Monthly reports, comparisons, trends, financial health, Smart Insights |
| Recurring costs | Expense rules, candidate detection, upcoming costs, reminders |
| Access | English, Ukrainian, Russian; Free/Premium access policies |
| Data controls | User-owned export and confirmed reset/deletion |

See [Features and scope](docs/FEATURES.md).

## Typical user journey

1. Open a private bot chat and choose a language.
2. Add income or an expense through guided entry or text input.
3. Review the amount and category, then confirm.
4. Set a category budget or savings goal and check progress.
5. Upload a supported CSV statement, review categories, and confirm the import.
6. Explore history, statistics, monthly reports, or Smart Insights.

This describes implemented workflows; no public live demo is provided here.

## Smart Insights

Local analysis of recorded activity highlights potential recurring costs, unusual expenses, category growth, repeated purchases, and illustrative savings opportunities. Reports indicate insufficient data where applicable. No mandatory external AI or paid analytics API is required.

Signals are observations, not proof of a subscription, guaranteed savings, or a complete financial picture. Private formulas and detection thresholds are excluded.

## Free / Premium concept

The private application includes feature access policies, premium entitlements, test billing, and Telegram Stars lifecycle infrastructure. These support a Free/Premium product concept with gated capabilities. Exact commercial policies and quotas remain private.

Real payments, revenue, paid conversion, and a launched commercial service are not claimed.

## Tech stack

- **Python** — application logic and local calculations.
- **aiogram 3** — asynchronous Telegram interaction handling.
- **SQLite** — financial records, planning, and application state.
- **python-dotenv** — private environment configuration.
- **zoneinfo / tzdata** — timezone support.
- **JSON locale catalogs** — English, Ukrainian, Russian UI.
- **unittest** — private offline regression suite.
- **Linux / Oracle Linux** — controlled beta deployment.

## Architecture

Telegram interactions pass through language and UX handling into finance, planning, CSV import, reporting, and access-policy components backed by SQLite. Imports require review and confirmation. Reporting reads stored activity; operational controls cover startup, backups, and safe logging.

See [High-level architecture](docs/ARCHITECTURE.md).

## Screenshots

No screenshots or public demo media are included. No image assets were found in the inspected project folders or source archive inventories. Future captures should use an isolated synthetic demo and pass privacy review. See [Asset guidelines](assets/README.md). No fabricated images are used.

## Release and quality assurance

- **Current status:** Beta 1.3.14 — Release Candidate / Beta Deployment.
- **Automated regression:** 454 automated tests passed, 0 skipped.
- Offline verification and normal, reverse, and randomized test-order runs passed.
- Deployment package structure validation passed.
- **Deployment context:** remote Linux beta deployment on Oracle Linux.
- **Multilingual UI:** UA / EN / RU (Ukrainian / English / Russian).

These results summarize the supplied Beta 1.3.14 release verification; tests were not rerun as part of this public documentation update.

**Pending before production readiness:** native Oracle Linux regression, Telegram live acceptance, and journal/service verification. This release remains a release candidate.

## Status and limitations

SmartSave is a pre-revenue technical product at the release-candidate stage for controlled beta deployment. This repository remains a documentation-only showcase; the private application and deployment package are not included.

- Single-process SQLite architecture; distributed operation and high-scale performance are not demonstrated.
- CSV supports defined formats and UAH amounts, without live bank synchronization or currency conversion.
- Duplicate protection applies to CSV imports and has documented edge cases.
- Reports and forecasts depend on the completeness of recorded data.
- Native Oracle Linux regression, Telegram live acceptance, and journal/service verification remain pending; real Stars payments are not verified here.
- Automated results above apply to Beta 1.3.14 and do not establish production readiness.

## Repository contents

```text
SmartSave-showcase/
|-- README.md
|-- .gitignore
|-- docs/
|   |-- ARCHITECTURE.md
|   |-- FEATURES.md
|   `-- SAFETY.md
`-- assets/
    `-- README.md
```

All repository text was written specifically for this showcase. Private source archives, financial records, configuration, and internal reports are excluded. See [Safety review](docs/SAFETY.md).
