# Commerce Intelligence Report

Interactive e-commerce analytics dashboard built with HTML, CSS and Chart.js.

**Live demo:** [commerce-intelligence-report.vercel.app](https://commerce-intelligence-report.vercel.app)

---

## About

Full analysis of 80,228 transactions from a Brazilian e-commerce operation (March-April 2021). Three-page interactive dashboard with real data, live filters and business storytelling.

**Pages:**
- Executive Overview — KPIs, daily revenue, department breakdown
- Market & Channels — geographic distribution, channel performance, card brand analysis
- Customer Profile — age distribution, income brackets, geographic origin

**Key findings:**
- R$72.6M in revenue over 15 days
- Top 4 departments account for 84% of total revenue
- Internet channel generates 19% higher average order value than Mobile
- SP + RJ + MG concentrate 73% of national sales volume
- 75+ is the largest customer age group

---

## Tech stack

- HTML / CSS / JavaScript — zero dependencies, no build step
- Chart.js 4.4 — data visualisation
- Google Fonts — Outfit + JetBrains Mono
- Vercel — hosting

---

## Dataset

Two source tables joined on `cliente_Log`:

| Table | Rows | Key columns |
|---|---|---|
| base compra | 80,228 | date, price, department, state, channel, card brand |
| Base cliente | 26,425 | age, income, state of birth |

---

## Run locally

```bash
open index.html
```

No server or build step required. All data is embedded in the HTML file.

---

Built by **Ingrid Martinez** — Data Analyst — Kilkenny, Ireland

[LinkedIn](https://www.linkedin.com/in/ingridmartinezm/) · [GitHub](https://github.com/martinez-ie) · [Portfolio](https://ingrid-martinez-portfolio.vercel.app/)
