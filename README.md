# multi-market-growth-os

An operating system for running one growth engine across several countries at once: a central strategy that sets the rules, and local teams that adapt them to each market's buyers, seasons, competitors and brand maturity.

## The problem

Expanding into a new country usually fails in one of two ways:

1. **Copy-paste.** Headquarters ships the home-market playbook unchanged. Messaging misses, channels that worked at home underperform, and budget is spread evenly across markets that are at very different stages.
2. **Fragmentation.** Every country runs its own show. Nobody can compare CAC across markets, wins never travel, and leadership loses the ability to move budget to where it earns the most.

The real question is not "how do we run marketing in country X". It is: **how do you build one growth engine that respects local nuance while still scaling regionally?**

## The model: global strategy, local execution

```
                 CENTRAL GROWTH STRATEGY (regional)
   positioning · core acquisition channels · paid efficiency rules
          measurement model · budget guardrails · test library
                               |
         +---------------------+---------------------+
         |                     |                     |
   MARKET A (launch)     MARKET B (traction)   MARKET C (scale)
   local intelligence:   local intelligence:   local intelligence:
   audience research,    seasonality, pain     buying journey,
   pain points by size   points by size        retention levers
```

The centre owns **what is the same everywhere**: positioning pillars, the channel toolkit, the metric definitions, the budget logic and the experiment library. Each market owns **what has to be different**: audience research, seasonality, pain points by customer size, local partners and the full-funnel journey as it actually happens in that country.

That split lets you:

- adapt messaging per country without rewriting the brand,
- prioritise channels (paid, CRM, events, sales enablement) differently per market,
- allocate budget by maturity stage instead of by headcount or habit,
- compare every market on the same scoreboard: CAC, ROI, revenue per market, conversion and channel efficiency.

## Structure

```
docs/
  01-central-vs-local.md            who decides what, with a RACI
  02-market-entry-checklist.md      gates from "should we enter" to "ready to scale"
  03-channel-prioritization-matrix.md  channels ranked by market maturity
  04-budget-model-by-stage.md       launch / traction / scale allocation logic
  05-measurement-plan.md            metric definitions, formulas and cadence
templates/
  country-playbook.md               one per market, owned locally
  weekly-market-review.md           30-minute cross-market review
  experiment-backlog.md             shared backlog, tagged by market
config/
  markets.example.yaml              markets, stages, channels and guardrails as data
examples/
  toolbase/                         a fictional marketplace expanding into three countries
```

## How to use it

1. **Set the centre first.** Fill in the central column of `docs/01-central-vs-local.md`: positioning pillars, channel toolkit, metric definitions. If those are not shared, nothing downstream is comparable.
2. **Classify each market** as `launch`, `traction` or `scale` using the criteria in `docs/04-budget-model-by-stage.md`, and record it in `config/markets.example.yaml`.
3. **Run the entry checklist** (`docs/02-market-entry-checklist.md`) for any market still in `launch`. Do not spend scale budget before the gates are green.
4. **Pick channels per market** with the matrix in `docs/03-channel-prioritization-matrix.md`. Each market should run two primary channels and at most two tests at a time.
5. **Write one country playbook** per market (`templates/country-playbook.md`). The local lead owns it; the centre reviews it quarterly.
6. **Run the weekly market review** (`templates/weekly-market-review.md`) on the shared scoreboard from `docs/05-measurement-plan.md`. Move budget between markets monthly, based on marginal CAC and payback, not on last month's split.
7. **Feed the backlog.** Every market logs tests in `templates/experiment-backlog.md`. A win in one market becomes a candidate test in the others.

See `examples/toolbase/` for the whole loop filled in for a fictional company.

## What it is not

- **Not a media plan.** It decides where money and attention should go; it does not choose keywords or creatives.
- **Not a localisation agency brief.** Translation is the smallest part of local execution.
- **Not a tool.** It works in a spreadsheet, a BI tool or a CRM. The YAML config is there so the rules can be versioned and reviewed, not because you need code.
- **Not for single-market companies.** If you only operate in one country, a standard growth model is enough.

## Case note

Built and ran a version of this to expand TUL, a B2B construction-supplies marketplace, into Colombia, Brazil and Mexico.

All numbers, markets and company names in this repository are illustrative.

## License

MIT, see [LICENSE](LICENSE).

---

Built by [Tadeo Lescano](https://www.linkedin.com/in/tadeo-lescano/), GTM Engineer & Growth Marketer. More at [github.com/tadeolescano](https://github.com/tadeolescano).
