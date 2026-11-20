# Experiment backlog (all markets)

One backlog for every market, so wins can travel. Score with ICE (impact, confidence, ease, each 1 to 10) and sort by score within each market. Anything that wins in one market gets a sibling row for the others with status `rollout-candidate`.

| ID | Market | Funnel stage | Hypothesis | Primary metric | Impact | Confidence | Ease | ICE | Status | Owner | Origin |
|---|---|---|---|---|---|---|---|---|---|---|---|
| MM-001 | | acquisition | If we [change], then [metric] will [move] because [reason] | | | | | | idea | | local |
| MM-002 | | activation | | | | | | | idea | | central |
| MM-003 | | retention | | | | | | | idea | | rollout of MM-0xx |

**ICE** = (impact x confidence x ease) / 10, rounded.

**Status values:** idea, scored, scheduled, running, won, lost, inconclusive, rollout-candidate, rolled-out.

**Rules**

- Every running test has a success threshold and a stop date written before launch.
- A market runs at most two tests on the same funnel stage at once.
- Inconclusive is a valid result. Log it, with the sample reached, so nobody reruns the same underpowered test.
