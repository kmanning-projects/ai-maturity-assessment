# Self-Assessment Tool

Two ways to run the assessment.

## v1 — Spreadsheet (now)
1. Open [`assessment.csv`](assessment.csv) in Excel or Google Sheets.
2. Score each of the five dimensions **1–5** using the rubric in [`../docs/maturity-model.md`](../docs/maturity-model.md).
3. Record the evidence in the Notes column — the score is only as good as the evidence behind it.
4. Compute the (optionally weighted) average, and **plot the five scores as a radar chart** (Insert → Chart → Radar).
5. Read the *shape*: your lowest high-leverage dimension is the binding constraint. Read its rubric one level up — that's your next investment.

## v2 — Web app (built ✅)
A no-backend static page ([`../index.html`](../index.html)) where you score the five dimensions with sliders and get an interactive radar chart + an auto-generated "binding constraint" diagnosis and next-level recommendation. Single file, Chart.js via CDN, zero cost.

- **Run locally now:** open `index.html` in any browser.
- **Publish free via GitHub Pages** (once the repo is public): Settings → Pages → Source: `main` / root, or:
  ```bash
  gh api -X POST repos/kmanning-projects/ai-maturity-assessment/pages -f 'source[branch]=main' -f 'source[path]=/'
  ```
  Then it's live at `https://kmanning-projects.github.io/ai-maturity-assessment/`. (GitHub Pages on a private repo requires a paid plan; make the repo public first.)

## Interpreting results
- **Average score** = a headline only. Don't lead with it.
- **The profile shape** = the insight. Uneven profiles (e.g. strong Data, weak Governance) are the norm and tell you exactly where to spend.
- **Binding-constraint rule:** raise the weakest *high-leverage* dimension by one level; stop over-investing in dimensions already ahead of the constraint.

See [`../docs/sample-report.md`](../docs/sample-report.md) for a worked diagnosis.
