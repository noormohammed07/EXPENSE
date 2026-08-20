# Chennai Finance Dashboard

An interactive personal-finance dashboard built from a monthly Excel expense ledger. Started as a plain spreadsheet (`data/chennai_expense.csv`) and rebuilt as a static, client-side dashboard — no backend, no build step, just open `index.html`.

**[Live demo →](#)** *(enable GitHub Pages on this repo to get a live link — see below)*

## What it shows

- **KPI strip** — total expense, savings, highest/lowest spending month
- **Monthly total expense** (bar) and **trend** (line) across Jan–Aug
- **Expense breakdown by category** (donut) and a ranked comparison (horizontal bar)
- **Filters** for month and category that cross-highlight every chart and update a plain-language insight line

## Data

`data/chennai_expense.csv` holds 9 categories tracked monthly: Rent, Food, Dress, Outing, Coffee & Tea, Travel, Hospital, Others, and EMI. The dashboard's dataset in `index.html` mirrors this file directly — swap in your own numbers to reuse it for a different month or city.

| Month | Total |
|---|---|
| January | ₹4,505 |
| February | ₹18,750 |
| March | ₹17,600 |
| April | ₹16,850 |
| May | ₹19,300 |
| June | ₹16,800 |
| July | ₹18,650 |
| August | ₹14,200 |

## Tech

- Plain HTML/CSS/JS — no framework, no bundler
- [Chart.js](https://www.chartjs.org/) (via CDN) for all charts
- Google Fonts: Fraunces (display), Inter (body), JetBrains Mono (data/labels)

## Run locally

Clone the repo and open `index.html` in a browser — that's it.

```bash
git clone https://github.com/<your-username>/chennai-finance-dashboard.git
cd chennai-finance-dashboard
open index.html   # or just double-click it
```

## Deploy on GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Source**, pick the `main` branch and `/ (root)` folder.
4. Save — your dashboard will be live at `https://<your-username>.github.io/chennai-finance-dashboard/` within a minute or two.

## Project structure

```
chennai-finance-dashboard/
├── index.html          # dashboard (HTML + CSS + JS in one file)
├── data/
│   └── chennai_expense.csv
└── README.md
```

## Why this project

Built to practice turning a raw spreadsheet into a data-driven, interactive front end — data modeling, chart libraries, and basic UI/UX in one small self-contained project.
