# Saint Mary's Offense — Coach's Dashboard (Design Prototype)

Interactive design prototypes for a coach-facing offensive analytics dashboard for the **Saint Mary's Gaels** 2025–26 men's basketball season.

> **Status:** Visual prototype with mock data. No real-data wiring yet.

---

## What's in here

Three design directions you can compare, plus a hub page to flip between them.

| File | Direction | Inspired by |
|---|---|---|
| `index.html` | Comparison hub with preview tiles | — |
| `variant_a_minimal.html` | Minimal editorial / list-led | Linear, Stripe, Vercel |
| `variant_b_cards.html` | Card grid with drill-in expansion | Figma, Notion, Stripe Atlas |
| `variant_c_dense.html` | Data-dense pro w/ sidebar | Synergy, InStat, Second Spectrum |

The active design direction is **Variant B**. Click any of the 5 segment cards (Transition, Early/Motion, Ball Screen, Half-Court Sets, Underneath OB) to expand into a drill-down view with breakdowns by trigger/action, top-performer portrait cards, and lineup analysis.

---

## Tech

Zero build step. Plain HTML + CSS + a tiny `<script>` for interactivity. Open the files directly in a browser.

- **Mock data** lives in `_shared/mock_data.js` — change a number once, see it everywhere
- **Logo** in `_shared/smc_logo.png`
- **Fonts** loaded from Google Fonts CDN (Inter)

---

## Run locally

Just open the hub page in a browser:

```bash
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows
```

Or serve via a quick local server:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

---

## Project structure

```
.
├── index.html               # Comparison hub
├── variant_a_minimal.html   # Minimal editorial direction
├── variant_b_cards.html     # Card grid direction (current focus)
├── variant_c_dense.html     # Data-dense pro direction
├── _shared/
│   ├── mock_data.js         # All sample data — players, lineups, segments
│   └── smc_logo.png         # SMC Gaels logo
└── README.md
```

---

## Feedback welcome

This is a design exploration. Click around, especially in Variant B → Transition card to see the full drill-down pattern. The other 4 segment cards (Early/Motion, Ball Screen, Half-Court Sets, Underneath OB) also drill in with the same pattern.

If you have thoughts on layout, hierarchy, color, motion, or what data should be surfaced — open an issue or send notes directly.
