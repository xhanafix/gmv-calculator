# TikTok GMV Max Budget & ROI Calculator

A single-page calculator for TikTok **GMV Max** ads campaigns — plan your ad budget and see profit, ROAS, and break-even numbers in real time.

Designed in a **Typography First** editorial style: one parchment-white scrolling page where the numbers are the hero, set in Fraunces and Space Grotesk with a single vermilion accent.

## Features

- **Live calculations** — results update instantly as you type (no button needed)
- **Profit per unit** before ads, plus **total revenue** and **total costs** (product + fees + commission)
- **Net profit** and **TikTok-style ROAS** (1–20 scale)
- **Break-even ROAS** — the score you must stay above to remain profitable
- **Break-even units** — how many pieces you must sell to cover your ad spend
- Footer stats: **visitor counter**, the visitor's **public IP**, and a TikTok link
- Color cues: green = profitable, red = losing money

## How the math works

| Input | Default |
| --- | --- |
| Selling price | RM 18.00 / pcs |
| Product cost | RM 6.00 / pcs |
| TikTok fee | 21% of sale |
| Affiliate commission | 10% of sale |
| Ad budget | user-defined |
| Units sold | user-defined |

```
Fees per unit   = selling price × (TikTok fee % + commission %)
Profit per unit = selling price − product cost − fees per unit
Net profit      = (profit per unit × units sold) − ad budget
ROAS            = (selling price × units sold) ÷ ad budget   (TikTok 1–20 scale)
Break-even ROAS = (ad budget + total product costs) ÷ ad budget
```

> Note: TikTok reports ROAS as a revenue multiplier (1–20), not a percentage. A ROAS above your break-even ROAS means the campaign makes money.

## Usage

1. Download `tiktok_gmv_calculator.html` (single file, no build step needed).
2. Open it in any modern browser (Chrome, Edge, Firefox, Safari).
3. Type your numbers — everything recalculates live.
4. The "Visitors" counter and "Your IP" row need an internet connection; if offline they show `–`.

## Hosting it live (free)

**GitHub Pages** — recommended, free, and permanent:

1. Create a new repository on GitHub (e.g. `gmv-calculator`).
2. Upload `tiktok_gmv_calculator.html` and this README to the repo.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to `Deploy from a branch`.
5. Choose branch `main` (or `master`) and folder `/ (root)`, then **Save**.

Your calculator will be live at:

```
https://<your-username>.github.io/gmv-calculator/
```

> Always push through `main`, and the site auto-rebuilds on every change. Files under `https://*.github.io` load fine over HTTPS, so the visitor counter and IP lookups work.

**Alternatives** (same single file): Vercel (`vercel` CLI or dashboard) or Netlify (drag-and-drop `tiktok_gmv_calculator.html`).

## Privacy

- The visitor counter uses a free third-party API ([counterapi.dev](https://counterapi.dev)).
- Your IP is looked up via [ipify.org](https://ipify.org) and shown to the visitor themselves; nothing is logged by this page.

## Made by

[@saya_hanafi](https://www.tiktok.com/@saya_hanafi) — TikTok GMV Max · Malaysia