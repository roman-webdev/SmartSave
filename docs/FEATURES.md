# Features and scope

Capabilities below are supported by inspected handlers, domain modules, UX routes, and product documentation. Implementation evidence does not imply a verified public deployment.

| Feature | User-facing behavior | Scope / limitation |
| --- | --- | --- |
| Income and expenses | Guided/text entry, preview, confirmation, editing | User-provided records; no live bank balances |
| Categories | Selection, review, learned categorization | User correction may be necessary |
| Accounts | Balances, reconciliation, linked transfers | Transfers excluded from income/expense totals |
| Budgets | Category limits, progress, alerts, forecasts | Depends on recorded data and access policy |
| Goals | Targets, optional dates, contributions, progress | Reflects recorded contributions |
| CSV import | Validation, preview, category review, confirmation/cancellation | Supported formats; UAH only, no conversion |
| Duplicate protection | Detect repeated imported entries within/across imports | Identical same-day entries can be treated as duplicates; earlier manual entries are not reconciled with CSV rows |
| History/statistics | Transaction review and summarized activity | Depends on entry/import completeness |
| Financial analysis | Monthly reports, comparisons, trends, financial health | Read-only calculations over stored activity |
| Smart Insights | Potential recurring costs, unusual expenses, growth, repeats, savings scenarios | Limited data can produce no signals; no guaranteed prediction or savings |
| Recurring costs | Rules, candidate detection, upcoming expenses, reminders | Candidates are suggestions, not confirmed subscriptions |
| Languages | English, Ukrainian, Russian; saved preference | Multilingual UI implemented |
| Data controls | Owned export and confirmed reset/deletion | No personal exports included |
| Free/Premium | Access policies, entitlements, test billing, Stars lifecycle | Real payments and revenue unverified |

## Import workflow

Upload a supported statement, inspect its normalized preview, review categories, then confirm or cancel. Transactions are saved after confirmation; import duplicate checks and original statement dates support accurate history and reporting.

No sample statements, fingerprint formulas, private scoring rules, or business-policy details are published.

## Evidence basis

The review used product/CSV documentation, architecture notes, declared dependencies, Telegram command handlers, planning functions, analytics components, and UX routes. Local audit/verification notes qualify readiness claims. Source archives were inventoried without extraction into this showcase.

No bot was started, no financial database was opened, and no tests were rerun for this documentation task. Earlier test results are not presented as fresh verification.
