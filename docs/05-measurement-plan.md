# Measurement plan

One scoreboard, one set of definitions, every market. If two markets calculate CAC differently, the comparison is worse than useless because it moves budget in the wrong direction.

## Core metrics

| Metric | Definition | Formula | Grain | Owner |
|---|---|---|---|---|
| CAC (blended) | Fully loaded cost to acquire one new paying customer | (media + agency fees + tools attributable to acquisition + acquisition team cost) / new paying customers | Market x month | Central growth |
| CAC (paid, by channel) | Media cost per new paying customer attributed to the channel | channel media spend / customers attributed to channel | Market x channel x month | Performance |
| Marginal CAC | Cost of the last customers acquired at the current spend level | delta spend / delta customers between two spend levels | Market x channel | Central growth |
| ROI | Return on growth spend over a defined window | (gross margin from new customers in window - growth spend) / growth spend | Market x quarter | Central growth + finance |
| CAC payback | Months of gross margin needed to recover CAC | CAC / (average monthly gross margin per new customer) | Market x cohort | Finance |
| Revenue per market | Net revenue booked from customers in the market | sum of net order value after returns and discounts | Market x month | Finance |
| New-customer revenue share | Share of market revenue from customers acquired in the period | revenue from new customers / revenue per market | Market x month | Central growth |
| Conversion rate (stage) | Share of entities moving from one funnel stage to the next | count at stage n+1 / count at stage n, within a fixed window | Market x stage x month | Market lead |
| Visit-to-lead | | leads / sessions | Market x channel | Performance |
| Lead-to-qualified | | qualified leads / leads | Market | Sales + market lead |
| Qualified-to-first-order | | first orders / qualified leads | Market | Sales |
| Channel efficiency | Revenue generated per unit of channel cost, normalised so channels are comparable | attributed new-customer gross margin (first 90 days) / channel cost | Market x channel x month | Performance |
| Repeat rate | Share of new customers placing a second order within 60 days | customers with 2+ orders in 60d / new customers | Market x cohort | CRM |

## Definitions that must be fixed centrally

- **New paying customer**: first completed and paid order, not sign-up.
- **Attribution model**: pick one (for example, position-based with a 30-day window) and use it in every market. Report a second view only as a sensitivity check.
- **Currency**: report in local currency and in one regional currency at a fixed planning rate for the year, so exchange-rate moves do not look like performance changes.
- **Cohort**: customers grouped by the month of their first paid order.
- **Fully loaded cost**: list exactly which cost lines are included and keep the list identical across markets.

## Dashboard layout

1. **Regional summary**: revenue per market, blended CAC, payback, ROI, against target, with month-on-month change.
2. **Market comparison**: the same five metrics side by side, plus stage.
3. **Channel efficiency by market**: matrix of markets x channels, coloured by efficiency against the band.
4. **Funnel by market**: stage conversion rates with the regional median as a reference line.
5. **Cohorts**: repeat rate and revenue retention by monthly cohort, per market.

## Data quality checks (weekly)

- Spend in the dashboard matches platform invoices within 2%.
- Share of new customers with no source captured is under 10% per market.
- No market has a funnel stage with more entities than the stage before it.
- Currency conversion uses the planning rate, not the daily rate.

## Cadence

| Report | Frequency | Audience |
|---|---|---|
| Market scoreboard | Weekly | Growth team, market leads |
| Budget reallocation pack | Monthly | Head of growth, finance |
| ROI and payback by cohort | Quarterly | Leadership |
