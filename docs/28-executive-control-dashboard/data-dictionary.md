# Dashboard Data Dictionary

## Workstream register

- `status`: proposed, not_started, in_progress, blocked, completed, on_hold.
- `planned_progress_pct`, `actual_progress_pct`: numeric percentage from 0 to 100.
- `owner`: accountable workstream lead.
- `blocker`: material dependency or obstacle; leave blank if none reported.

## Budget control

All monetary fields are IDR amounts, entered as plain numbers without currency
symbols or thousands separators.

- `budget_idr`: approved budget, not an unapproved estimate.
- `committed_idr`: authorized contractual or purchase commitments.
- `actual_idr`: recognized actual expenditure.
- `forecast_at_completion_idr`: latest expected total cost at completion.

Do not aggregate different currencies without a documented conversion method.

## Funding register

Use explicit statuses such as `proposed`, `under_review`, `conditionally_approved`,
`confirmed`, `received`, `rejected` or `cancelled`.

`confirmed` should be used only when documentary evidence and authorized
approval have been checked. Confirmation does not mean the funds are available
as cash.

`received` requires evidence of receipt and completed reconciliation. Record
the evidence in `evidence_reference` and `verified_date`; record the
reconciliation artifact in `reconciliation_reference` and its completion date
in `reconciliation_date`. These references must point to controlled records
that an authorized reviewer can access.

A verbal promise, indicative term sheet, proposed investment, or conditional
approval is not received funding. Do not report it as cash received or cash
available. An amount with missing evidence or reconciliation must be flagged
as incomplete and excluded from the verified-received total.

## Risk register

- `likelihood` and `impact`: integer scores from 1 to 5.
- `status`: open, mitigating, accepted, closed.
- Record a named owner and due date for material risks.

## Decision log

- `status`: pending, in_review, approved, rejected, deferred, completed.
- Decisions should have a clear owner and due date.

## KPI register

- `target` and `actual`: numeric values using the unit declared in `unit`.
- Keep each KPI's unit and reporting period consistent when comparing values.
- Define source evidence and calculation method in the KPI governance record.
