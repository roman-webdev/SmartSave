# Features and scope

SmartSave Beta 1.3.14 is a Release Candidate / Beta Deployment with a multilingual UA / EN / RU interface. The table summarizes user-facing capabilities; it does not establish production readiness.

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

## Release verification and scope

The supplied Beta 1.3.14 release verification reports **454 automated tests passed, 0 skipped**, covering offline verification and normal, reverse, and randomized test-order runs. Deployment package structure validation passed.

Linux / Oracle Linux is the controlled beta deployment context. **Native Oracle Linux regression, Telegram live acceptance, and journal/service verification remain pending before production readiness.**

No bot was started, no financial database was opened, and no tests were rerun for this public documentation update. Private source, internal reports, and deployment instructions remain excluded.
