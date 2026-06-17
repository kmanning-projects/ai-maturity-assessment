# Sample Diagnostic — "Northwind Financial"

A worked assessment showing how the model turns five scores into a single, fundable next move.

> **Northwind Financial** — a regional bank, ~5,000 employees, regulated. Leadership believes they're "behind on AI" and is tempted to fund a large model-platform buildout.

## Scores

| Dimension | Score | One-line rationale |
|-----------|------:|--------------------|
| Data & Infrastructure | **4** | Strong data warehouse, governed pipelines, cloud platform in place |
| Talent & Skills | **3** | A capable central data-science team; literacy thin outside it |
| Governance & Risk | **2** | Ad hoc reviews; no risk-tiering; shadow GenAI use in branches |
| Adoption & Process | **2** | Several pilots, almost nothing in production; low trust |
| Strategy & Funding | **3** | Stated ambition + some portfolio thinking; funding still project-by-project |

**Average: 2.8** — but the average is the least useful number here.

## The profile (shape > average)
```
Data & Infra      ████████░░  4
Talent & Skills   ██████░░░░  3
Governance        ████░░░░░░  2   ◀ binding constraint (high leverage, regulated)
Adoption          ████░░░░░░  2   ◀ second constraint
Strategy/Funding  ██████░░░░  3
```

## Diagnosis
Northwind's instinct — buy a bigger model platform — would pour money into **Data & Infrastructure, already their *strongest* dimension (4)**. That's the classic mistake the average score hides.

The **binding constraint is Governance (2)**, made high-leverage by their regulated context: until there's risk-tiered intake and oversight, nothing can safely reach production — which is exactly why **Adoption is also stuck at 2**. Strong data feeding ungoverned pilots that never ship is the whole problem in one sentence.

## Recommended next move
**Raise Governance from 2 → 3 first**, and pair it with an Adoption push:
1. Stand up a **risk-tiered intake + AI policy + model documentation** (see the [Governance Playbook](https://github.com/kmanning-projects/responsible-ai-governance)). This unblocks production, not just compliance.
2. Pick **2–3 stalled pilots** and shepherd them through the new governance to production with measured value — moving Adoption 2 → 3.
3. **Do not** fund the platform expansion this cycle; Data/Infra is already ahead of the constraint. Revisit once Governance and Adoption catch up.

**Expected effect:** unblocking the binding constraint converts existing (already-funded) data strength into shipped value — a far higher return than buying more infrastructure they can't yet safely use.

---
> **The lesson:** "Are we behind?" produces a platform purchase. "Which dimension is our binding constraint, and what does the next level cost?" produces a governance program that unlocks everything already built. Same budget; very different outcome.
