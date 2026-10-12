# Business KPI Dashboard – Customer Churn

**Live dashboard:** PASTE-YOUR-PUBLIC-LINK-HERE

An interactive dashboard that shows who is leaving, how much monthly revenue is at risk, and which customer groups to focus on.

## Files
- `churn_dashboard.html` – the dashboard (open in any browser)
- `customer_churn_sample.csv` – the cleaned customer churn dataset (15 customers, synthetic)
- `screenshot.png` – picture of the dashboard

## KPI definitions
- **Churn rate** = customers who left ÷ all customers × 100
- **Retention rate** = 100 − churn rate
- **Revenue at risk** = total monthly charges of customers who churned
- **Tenure** = average number of months a customer has stayed

## Filters
Contract type, tenure (0–12, 13–24, 25–36, 37+ months), and payment method.

## Charts
Bar charts for churn rate by contract, tenure and payment method, and revenue at risk by plan. Labels are on every chart, and the blue/orange colors are colorblind-safe.

## Key findings
- Churn rate is 47% (7 of 15 customers); retention is 53%.
- Revenue at risk is about $410 per month.
- All customers who left were on month-to-month contracts. No yearly-plan customer left.
- Customers who left stayed about 7 months on average, versus about 29 for those who stayed.

## Recommendation
Offer discounts or perks to move month-to-month customers to yearly plans, and check in with new customers during their first 12 months.

*Note: the dataset is small, so these patterns are a demonstration, not proof.*
