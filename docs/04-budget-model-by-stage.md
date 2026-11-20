# Budget model by stage

Budget follows evidence. A market earns more money by proving it can turn money into customers at an acceptable cost, not by having a larger team or a louder lead.

## 1. Set the regional envelope

Start from the total growth budget for the period. Reserve a fixed share before splitting by market:

| Bucket | Share of total | Purpose |
|---|---|---|
| Market budgets | 75 to 80% | Distributed by stage (below) |
| Central test fund | 10 to 15% | New channels and cross-market tests, allocated by the head of growth |
| Central infrastructure | 5 to 10% | Tracking, tools, shared creative production, research |

## 2. Allocate by stage, not evenly

Each market gets a stage weight. A market's share of the market budgets is its weight divided by the sum of all weights.

| Stage | Weight | Spend posture | Primary objective |
|---|---|---|---|
| Launch | 1 | Fixed, capped. Spend to learn, not to grow. | Find two channels with CAC inside the launch band |
| Traction | 2 to 3 | Grows month on month if gates hold | Bring CAC to target, prove retention |
| Scale | 4 to 5 | Variable, driven by marginal CAC | Maximise new revenue at target payback |

Example with three markets (one per stage) and 100 units to distribute: weights 1 + 3 + 5 = 9, so launch gets 11, traction 33, scale 56.

## 3. Split inside a market

| Stage | Primary channels | Test channels | Always-on support (CRM, retargeting, content) |
|---|---|---|---|
| Launch | 50% | 30% | 20% |
| Traction | 60% | 20% | 20% |
| Scale | 65% | 10% | 25% |

## 4. Reallocate monthly with marginal CAC

Average CAC hides saturation. Each month, for every market and primary channel, estimate the CAC of the **last** block of spend (for example the last 20%), using spend steps, geo holdouts or the response curve from the previous months.

Rules of thumb:

- If marginal CAC is under the target band and capacity exists, move money **in**.
- If marginal CAC is above the band for two months, move money **out**, even if average CAC still looks fine.
- Never move more than 20 to 25% of a market's budget in a single month; the learning phase on most paid platforms resets.

## 5. Guardrails

| Guardrail | Typical setting |
|---|---|
| Launch budget cap per market | Fixed amount per quarter, agreed at gate 0 |
| Maximum CAC payback | Set by finance (e.g. 12 months for B2B with good retention) |
| Minimum test budget | Enough to reach the success threshold within the stop date |
| Kill switch | CAC above two times band for three months with no improving trend |

## Worked formula

```
market_share_m   = weight_m / sum(weights)
market_budget_m  = market_budgets_total x market_share_m
channel_budget_c = market_budget_m x split[stage_m][channel_role_c] / channels_in_role
```

All percentages above are starting points. Calibrate them with your own payback and retention data after two or three cycles.
