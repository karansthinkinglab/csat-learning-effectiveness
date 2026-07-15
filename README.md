# CSAT & Learning Effectiveness Diagnostic

An interactive diagnostic analysing learner satisfaction across 14 global markets, built to answer one question: **is a rising average actually good news?**

> **Note:** This project uses fully synthetic data. Markets, scores, and root causes are illustrative and do not represent any real organisation, team, or individual.

---

## The finding

Global learner satisfaction was reported as a single average — 7.8, up 0.6 on the prior period. The headline looked healthy.

It wasn't. The average concealed a **2.9-point spread** between the strongest market (UK, 9.1) and the weakest (Japan, 6.2), and that spread was *widening* even as the mean improved. Three markets sat below the 7.5 target and were getting quietly worse.

## Problem

Learner satisfaction was tracked as a global mean. A rising mean invited a "no action needed" read, so declining markets went unnoticed and L&D had no signal on where to intervene or why.

## Approach

The diagnostic reads the same data as a **distribution rather than a mean**, and is structured on the **Kirkpatrick evaluation model** so each section answers a different level of the question:

| Level | Question | What the analysis shows |
|---|---|---|
| **L1 — Reaction** | Are learners satisfied? | CSAT trend by quarter, global vs top vs lowest market |
| **L2 — Learning** | Is the content landing? | Score distribution by programme type |
| **L3 — Behaviour** | Where is it breaking down? | Root cause per at-risk market |
| **L4 — Results** | What should change? | Recommendations sequenced by gap closed |

The key move is at L2: breaking scores down by **programme type** showed the weakness was in compliance and tech-skills content, not in particular geographies. The at-risk markets simply over-index on the weakest programmes. That reframes the problem from "these regions are underperforming" to "this content needs fixing" — which is actionable.

## Key results

- **2.9-point gap** between best and worst market, invisible in the 7.8 average
- **3 markets below target** (Mexico 6.8, Brazil 6.4, Japan 6.2), each traced to a specific, fixable content cause
- Weakness isolated to **compliance (7.3)** and **tech skills (7.0)** programmes, vs onboarding at 9.1
- Recommendation to **report spread alongside average**, so future divergence surfaces early rather than after a decline

## Why an interactive artifact, not a BI dashboard

This is a one-off **diagnostic narrative for a leadership audience**, not an operational monitoring tool. It has a beginning, a middle and a conclusion, and it stops being useful once the recommendations are actioned.

That made a self-contained web artifact the right tool: fast to produce, shareable by link, readable on any device, and with no BI licence or login required to open it. A Power BI or Tableau build would have added overhead without adding anything the argument needed. (For genuinely operational, recurring monitoring, I use Power BI and Tableau — see my other projects.)

---

## Repository contents

```
csat-learning-effectiveness/
├── README.md
└── csat_learning_effectiveness.html   # self-contained interactive diagnostic
```

## How to view

Download `csat_learning_effectiveness.html` and open it in any browser. No build step, no dependencies to install — Chart.js loads from a CDN and the synthetic dataset is inline.

## Tools

HTML · CSS · JavaScript · Chart.js · Claude
