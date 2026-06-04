# Self-Assessment Tool

Two ways to run the assessment.

## v1 — Spreadsheet (now)
1. Open [`assessment.csv`](assessment.csv) in Excel or Google Sheets.
2. Score each of the five dimensions **1–5** using the rubric in [`../docs/maturity-model.md`](../docs/maturity-model.md).
3. Record the evidence in the Notes column — the score is only as good as the evidence behind it.
4. Compute the (optionally weighted) average, and **plot the five scores as a radar chart** (Insert → Chart → Radar).
5. Read the *shape*: your lowest high-leverage dimension is the binding constraint. Read its rubric one level up — that's your next investment.

## v2 — Web app (planned)
A no-backend static page (GitHub Pages) where you answer 15 questions and get an interactive radar + auto-generated recommendations. Built with Claude Code, hosted free. Tracked as a stretch goal in the [spec](https://github.com/kpandkm-projects/ai-strategy-operating-model).

## Interpreting results
- **Average score** = a headline only. Don't lead with it.
- **The profile shape** = the insight. Uneven profiles (e.g. strong Data, weak Governance) are the norm and tell you exactly where to spend.
- **Binding-constraint rule:** raise the weakest *high-leverage* dimension by one level; stop over-investing in dimensions already ahead of the constraint.

See [`../docs/sample-report.md`](../docs/sample-report.md) for a worked diagnosis.
