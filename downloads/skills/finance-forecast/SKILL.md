---
name: finance-forecast
description: Build an evidence-based twelve-month expense forecast with explicit assumptions and cancellation scenarios.
---

# Finance forecast

Use when asked to forecast spend from a classified transaction ledger. Read actual saved transactions or use the Finance Manager forecast_spending tool. Never invent figures or claim a forecast is certain.

1. Reconcile row counts, amount totals, currencies and time coverage against the source statements. Preserve refunds. Exclude transfers, confirmed personal charges and explicitly excluded duplicate charges from business spend. Keep unresolved rows visible; state how they affect completeness.
2. Identify recurring commitments from multiple observed billing months. Use invoices/contracts for cadence when available. Separate annual renewals from monthly subscriptions. A merchant's recurrence does not establish future obligation; mark inference.
3. Use the last six available calendar months of non-recurring business expenses as the variable baseline. Missing months are missing data, not automatically zero. Require sufficient history or explain the reduced basis.
   When at least two complete calendar years exist, calculate each calendar month’s variable-spend index relative to its own year’s monthly average, average those indices across complete years, and apply it to the recent variable baseline. Otherwise use the flat baseline and disclose insufficient seasonal history. Do not add random variation. Assume the latest statement month is complete only if the user confirms it.
4. Project the next twelve months after the most recent statement. Add monthly commitments and annual renewals in their observed renewal month. Apply user-provided annual growth to variable spending, default 0%, compounding monthly. Show the assumption.
5. Produce baseline and cancellation scenarios. Monthly cancellation savings start next month; annual savings start at the next renewal. State that actual notice periods, minimum terms, taxes, refunds and replacement costs can change savings. Never execute a cancellation.
6. Show monthly totals and annual totals, delta, assumptions, data cutoff and source IDs. Explain the largest drivers. Offer a sensitivity range by changing growth/commitments, not an invented statistical confidence interval.
7. If sufficient history exists, backtest a specified baseline on held-out months without future leakage. Name the baseline and metric. The app's displayed three-month WAPE evaluates a simple trailing-six-month average; it is not a calibration score for the full recurring-commitment projection.
8. Label outputs from supplied data “Synthetic demonstration.” Show missing evidence and suggest the next useful input. Return editable assumptions and a CSV/JSON export.
