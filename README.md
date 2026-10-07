# Customer Churn KPI Dashboard

This submission is a single-file interactive dashboard built from the supplied cleaned customer churn dataset.

## KPI definitions
- **Churn rate:** churned customers / customers in the current filter.
- **Retention rate:** 1 - churn rate.
- **Revenue at risk:** sum of monthly charges for churned customers in the current filter. This is **monthly** revenue at risk, not an annual forecast.
- **Tenure KPI:** average completed tenure in months.

## Filters
- Contract
- Tenure band: 0–6, 7–12, 13–24, 25+ months
- Payment method

## Data quality checks
- 15 customer records.
- No missing values.
- No duplicate customer IDs.
- Observed ranges: age 23–60, tenure 2–48 months, monthly charge ₹49.99–₹149.99, support tickets 0–6.
- No rows were silently deleted.

## Baseline findings from the full sample
- Churn: 7/15 = 46.7%
- Retention: 8/15 = 53.3%
- Monthly revenue at risk: ₹409.93
- Average tenure: 18.8 months
- All 7 churned customers are on month-to-month contracts in this small sample.

## Decision framing
**Audience:** subscription retention/customer-success team.

**Decision:** prioritize customer groups with high observed churn and/or high monthly revenue at risk for outreach.

**Uncertainty:** this is a 15-customer fictional sample. The dashboard is descriptive and does not establish causation or predictive performance.

**Next measurement:** repeat the KPI analysis on a larger rolling cohort and track post-outreach churn, renewal, and retained monthly revenue.

## How to publish
Upload `customer_churn_dashboard.html` to a GitHub repository with GitHub Pages enabled, or to another static hosting service. The HTML is the proof page; no build step is required.
