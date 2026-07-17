# Team Cartier Dashboard

A financial-performance dashboard built for a business case competition. It visualizes a FY2024 wholesale-distribution P&L: forecast versus actual, budget variance, and working-capital investment.

## What it shows

- **KPI strip:** total and net revenue, gross profit, operating expenses, operating income, and net margin, each with year-over-year change.
- **Revenue by channel** and a forecast-vs-actual comparison across all channels (Warehouse, Direct, Storage).
- **P&L waterfall** bridging revenue to operating income, with GP and operating-income margins.
- **Top expenses vs budget** and **GP margin by channel** (forecast, actual, and norm).
- **Net investment** view of working-capital components (AR, AP) and an **expense-ratio scatter** flagging categories running over norm.

Figures shown (for example $15.3M revenue, 25+ expense categories) are the case-competition dataset, not live company data.

## Stack

A single static `index.html` with charts rendered by Chart.js loaded from a CDN. No build step is required to view it.

Note: `package.json` still lists a Create React App / react-scripts setup, but the actual dashboard in this repo is the standalone `index.html`; there is no React source.

## Run it

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8080
```

Then visit http://localhost:8080.
