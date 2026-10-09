# Eduardo Moreno

I’m a software engineer and the founder of **[TickerTrac](https://tickertrac.com)**, a product that helps investors revisit their investment theses as public evidence changes.

I build and operate the system across data ingestion, retrieval, model evaluation, background processing, and the application itself. My engineering work focuses on making AI judgments useful, traceable to their sources, and economical to run.

## Selected engineering work

### 1. Finding where AI judgment quality breaks

**1,000 cases · 3,600 model comparisons**

A production quality investigation revealed failures at several stages: source coverage, model judgment, citations, and delivery. I separated those failure types, compared interventions, and changed model routing by source type.

The work also rejected a seemingly cleaner prompt because it missed useful alerts. The resulting decisions addressed specific observed failures, with the evaluation’s limitations documented alongside the results.

**Demonstrates:** production diagnosis, evaluation design, model routing, and decisions grounded in evidence.

[Read: When better evidence changes the answer →](https://tickertrac.com/engineering/evidence-quality)

### 2. Improving retrieval—and checking the answers it produces

**100 cases · 20 companies**

I compared dense, hybrid, and reranked retrieval on a frozen, human-adjudicated corpus. Improved ranking exposed another problem: relevant evidence could still be missed across source collections.

The study follows the selected approach through answer review, a targeted coverage repair, and production rollback checks. It also records the nine answer cases that still failed at least one review criterion.

**Demonstrates:** retrieval engineering, benchmark design, source coverage, and validation beyond a single score.

[Read: Dense vs. hybrid retrieval →](https://tickertrac.com/engineering/retrieval-bakeoff)

### 3. Rejecting a cheaper model when the evidence does not support it

**3,169 retained judgments · 1,200 articles**

I evaluated a fast, inexpensive decision-only model for two roles: screening news and judging its relevance. Neither role met the agreement thresholds established before the experiment, so the candidate was not adopted.

The study preserves the unsuccessful result and distinguishes agreement with existing judgments from independently established correctness.

**Demonstrates:** disciplined experimentation, cost–quality tradeoffs, and a defensible decision to leave production unchanged.

[Read: Can a decision-only model judge news relevance? →](https://tickertrac.com/engineering/jev-judge-agreement)
