# Executive Control Dashboard

## Purpose

Provide a consolidated management view of project delivery, financial control,
funding status, enterprise risks, KPIs and pending executive decisions.

## Dashboard

Open `dashboard/index.html` in a modern browser. Upload the corresponding CSV
registers from `templates/executive-dashboard/` to view their current contents.

The dashboard processes uploaded CSV files locally in the browser. It does not
connect to bank systems, external funding providers, or live project databases.

## Data sources

| Dataset | Source template | Primary purpose |
|---|---|---|
| Workstreams | workstream-register.csv | Delivery status and progress |
| Budget | budget-control.csv | Budget, commitments, actuals and forecast |
| Funding | funding-register.csv | Funding pipeline and verification |
| Risks | risk-register.csv | Enterprise risk monitoring |
| Decisions | decision-log.csv | Outstanding management decisions |
| KPIs | kpi-register.csv | Target versus actual performance |

## Reporting rules

- Blank values mean not reported; they must not be interpreted as zero.
- Funding is confirmed only after documentary verification and authorized approval.
- Budget, committed expenditure, actual expenditure and forecast costs are separate measures.
- Every material KPI should have an owner, reporting period and evidence source.
- Status definitions must be standardized before management reporting.
- Do not upload confidential banking credentials, account details or unnecessary personal data.

## Recommended review cadence

- Weekly: delivery progress, blockers, decisions and high-priority risks.
- Monthly: financial close, budget variance, cash flow, KPI performance and funding verification.
- At each stage gate: evidence review, approval, conditions and recorded decision.

## Current limitations

This is a local CSV-driven dashboard prototype. It does not provide authentication,
role-based access, a database, audit logging, automatic CSV synchronization or
live financial integrations. Uploaded files remain in the browser session and
must be selected again after a reload.

The dashboard must not be treated as proof of funding, regulatory approval,
project completion or investment feasibility.
