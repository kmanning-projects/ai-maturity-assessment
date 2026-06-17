# The AI Maturity Model I Use to Diagnose Any Organization

*"Are we behind on AI?" is the wrong question — and it leads to expensive answers. Here's the five-dimension model I use instead, plus a free tool that finds the one thing actually holding you back.*

---

Every executive team asks me some version of the same question: *"Are we behind on AI?"* It feels like the responsible thing to ask. It's also almost useless — because it produces an answer like "yes, probably," which leads to an action like "let's buy a bigger AI platform," which is frequently the exact wrong move.

The better question is: **"Which dimension is our binding constraint, and what does the next level cost?"** That one produces a fundable, specific next move. To answer it, you need a model that scores maturity per *dimension* — because the average score hides the constraint, and the constraint is the only thing that matters.

## Five dimensions, five levels

I assess organizations across five dimensions, each rated Level 1 (ad hoc) to Level 5 (transformative):

1. **Data & Infrastructure** — can we feed and run AI reliably?
2. **Talent & Skills** — do we have the people, and is the org getting smarter?
3. **Governance & Risk** — can we deploy AI safely and defensibly?
4. **Adoption & Process** — does AI actually change how work gets done?
5. **Strategy & Funding** — is there a managed, funded plan, or a wish?

The levels follow a consistent shape: **Ad hoc → Emerging → Operational → Systemic → Transformative.** Level 2 is pilots with no repeatability. Level 3 is repeatable, measured delivery with some governance. Level 4 is a portfolio that's managed, governed, and funded. Most organizations cluster around Level 2 overall — and, crucially, they're *uneven*: a Level-3 data org stuck at Level-1 governance is completely typical.

That unevenness is the entire point. Here's why.

## The average lies. The shape tells the truth.

Consider a real-shaped example — call it **Northwind Financial**, a regional bank convinced it's behind and tempted to fund a large model-platform buildout. We score it:

```
Data & Infra      ████████░░  4
Talent & Skills   ██████░░░░  3
Governance        ████░░░░░░  2   ◀ binding constraint
Adoption          ████░░░░░░  2   ◀ second constraint
Strategy/Funding  ██████░░░░  3
```

Average: 2.8. If you lead with that number, you learn nothing. Look at the *shape* and the diagnosis is obvious.

Northwind's instinct — buy more infrastructure — would pour money into **Data & Infrastructure, which is already their strongest dimension (4).** That's the classic mistake the average hides.

Their actual binding constraint is **Governance (2)** — and in a regulated bank, governance is high-leverage: until there's risk-tiered intake and oversight, nothing can safely reach production. Which is *exactly why Adoption is also stuck at 2.* Strong data feeding ungoverned pilots that never ship is the whole problem, in one sentence.

## The binding-constraint rule

So the recommendation isn't "improve everything." It's surgical:

> Raise your weakest *high-leverage* dimension by one level. Stop over-investing in dimensions already ahead of the constraint.

For Northwind: stand up governance (risk tiering, an AI policy, model documentation) to move Governance 2 → 3 — which unblocks production — and shepherd two or three already-built pilots through it to move Adoption 2 → 3. Explicitly *do not* fund the platform expansion this cycle; Data/Infra is already ahead of the constraint.

Same budget. Completely different outcome. One path buys infrastructure they can't yet safely use. The other converts existing, already-funded data strength into shipped value. That's what a maturity model is *for* — not benchmarking your ego against competitors, but finding the one investment that unlocks everything else.

## Why "next level" beats "best practice"

Maturity models often fail because they hand you a Level-5 picture and an implicit instruction to go become Google. That's not actionable. The useful move is always **one level up on the constraint.**

If your Governance is at Level 2 (ad hoc reviews, informal rules), Level 3 is concrete: a risk-tiered intake, a written policy, model documentation. That's a quarter of work, not a five-year transformation. You raise the constraint, the next-weakest dimension becomes the new constraint, and you repeat. Maturity is a sequence of single steps on the binding constraint — not a leap to the summit.

## Try it on your own org

I built a free, no-login web tool that runs this assessment: score the five dimensions with sliders, and it draws your radar profile, identifies your binding constraint (lowest score, broken by leverage), and tells you what the next level concretely looks like for that dimension. It also flags the dimensions you're *over-investing* in relative to your constraint — the spending most orgs never question.

It's a single static page; nothing leaves your browser. The full rubric (all five dimensions × five levels, with evidence signals) and the Northwind worked example are open-source alongside it.

## The takeaway for leaders

Stop asking "are we behind?" It produces a platform purchase. Start asking "which dimension is our binding constraint, and what does the next level cost?" It produces a focused program that unlocks the value you've already paid for.

Most organizations are over-invested in models and infrastructure while stuck at Level 2 on governance and adoption — the two dimensions that actually convert capability into shipped value. A good maturity model makes that impossible to ignore.

---

*The rubric, the worked example, and the interactive assessment tool are open-source here: [github.com/kmanning-projects/ai-maturity-assessment](https://github.com/kmanning-projects/ai-maturity-assessment).*

*I'm a strategist who builds. If you're diagnosing where your organization actually stands on AI — and what to do about it — let's connect.*
