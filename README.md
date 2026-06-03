# Saint Mary's Offense — Coach's Dashboard

Interactive coach-facing offensive analytics dashboard for the **Saint Mary's Gaels** 2025–26 men's basketball season.

> **Status:** Visual prototype with mock data. Real-data wiring coming later.

---

## What's in here

| File | Purpose |
|---|---|
| `index.html` | **The dashboard** — main view (5 segment cards + drill-down) |
| `variants_hub.html` | Side-by-side comparison of three design directions explored early on |
| `variant_a_minimal.html` | Alternate design direction — Minimal Editorial |
| `variant_c_dense.html` | Alternate design direction — Data Dense Pro |
| `_shared/mock_data.js` | All sample data — players, lineups, segments |
| `_shared/smc_logo.png` | SMC Gaels logo |

---

## How to use

Click any of the 5 segment cards (Transition · Early/Motion · Ball Screen · Half-Court Sets · Underneath OB) to expand into a drill-down view with:

- Four Factors strip (PPP / Possessions / eFG% / TO% / OREB% / FT Rate)
- First-layer breakdown (triggers, actions, screens, or plays — varies per segment)
- Top Performers (player portrait cards)
- Lineup Analysis (scrollable 5-man unit performance)
- Filter pills above the breakdown for Ball Screen (coverage) and Half-Court (package)

Use the season timeline at the top to filter to specific games, wins/losses, conference, or by month.

---

## Tech

Zero build step. Plain HTML + CSS + a tiny `<script>` for interactivity.

---

## Run locally

```bash
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows
```

Or via a quick local server:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

---

## Feedback welcome

Click around, especially into the **Transition** card to see the full drill-down pattern. All 5 segment cards drill in the same way. Layout, hierarchy, color, motion, what data should be surfaced — all feedback welcome.
