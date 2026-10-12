# Recommendation Memo – Customer Churn Risk

**Data:** 15 customers (47% churned). Treat everything below as a *first signal*, not proof.

## What we found
- **Contract type is the strongest signal.** All 7 Month-to-Month customers churned; none of the 8 One Year / Two Year customers did.
- **New customers with many tickets are the clearest risk group.** The "New & Frustrated" segment (6 customers) averages about 6 months of tenure and 4.5 support tickets, and all of them churned.
- **Loyal Long-Term customers (Two Year, avg. 38 months) show no churn** and almost no tickets.
- **The risk score separates the groups.** Low-risk: 0 of 8 churned. Medium: 1 of 1. High: 6 of 6.
- **Revenue exposure:** Medium and High risk customers are 32% of monthly revenue ($409.93 of $1,269.85 in this sample).

## Recommendations (cautious)
1. **Contact High-risk customers first** (score 5+): a proactive call or a short onboarding check-in within the first 3 months.
2. **Fix the support experience for new customers.** Customers with 4+ tickets in their first year deserve a faster, personal follow-up.
3. **Test a small incentive** (e.g. a discount) for moving Month-to-Month customers to a One Year plan. Run it as an experiment before rolling out widely.
4. **Keep monitoring Loyal Long-Term customers.** The score can under-rate an unhappy long-term customer, so watch for ticket spikes.

## Limits
- Only 15 rows. The perfect separation is partly because the sample is tiny and tidy; a real dataset will be messier.
- The score was designed on the same data it was checked on, so accuracy is likely overstated.
- Correlation is not causation: month-to-month customers may leave because of pricing, competitors, or need, not the contract itself.
- Next step: re-test the score on a larger, newer set of customers and adjust the points.
