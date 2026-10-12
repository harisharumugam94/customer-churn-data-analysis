# Customer Churn: Data Quality and Exploratory Analysis

**Dataset:** synthetic customer churn sample (15 customers, 11 columns).

## Files
- `churn_analysis.xlsx`: full workbook (Clean Data, Data Quality Log, Summary Stats, Churn Patterns, Data Dictionary)
- `customer_churn_raw.csv`: original file
- `customer_churn_cleaned.csv`: cleaned file
- `data_dictionary.csv`: meaning of every column

## 1. Profiling
No missing values, no duplicate rows or CustomerIDs, correct data types, no extreme outliers
(Age 23-60, MonthlyCharges 49.99-149.99, SupportTickets 0-6).

## 2. Cleaning and validation
No changes were needed, so the cleaned CSV is identical to the raw CSV.
Assumptions checked (all passed):
- Customers are adults (age 18-100).
- No negative tenure, charges, or ticket counts.
- TotalCharges = TenureMonths x MonthlyCharges for every row.
- Churn and Gender contain only their expected values.
- Each subscription plan has one price.

## 3. Findings
- 7 of 15 customers churned (47%).
- All Month-to-Month customers churned; no One Year or Two Year customer did.
- Churned customers: younger (avg 30 vs 47), shorter tenure (7 vs 29 months), more support tickets (4.3 vs 1.0).

## Limitation
Only 15 rows, so these patterns are early hints, not proof.
