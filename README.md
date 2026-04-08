# Commerce Intelligence Report

> Interactive management dashboard analysing 80,228 e-commerce transactions across Brazil - built to answer the business questions that drive revenue strategy.

**[Live Demo](https://powerbi-dashboards-three.vercel.app/)** · [GitHub](https://github.com/martinez-ie/powerbi-dashboards)

---

## Business Questions This Project Answers

This dashboard was designed around the questions a commercial team actually asks - not just the metrics that are easy to build.

**Revenue strategy**
- Which product categories are generating the most revenue, and how concentrated is that dependency?
- Is the business over-reliant on a small number of departments, and what is the risk of that?
- What is the true cost of the free shipping policy as a percentage of total revenue?

**Channel and acquisition**
- Does the sales channel affect how much customers spend per transaction?
- Which channel should receive more acquisition budget to maximise revenue per transaction - not just volume?
- How significant is the gap between Mobile and Internet in average order value, and what does that mean for campaign allocation?

**Geographic expansion**
- Where is the business geographically concentrated, and which states represent untapped market opportunity?
- How does SP domination skew the overall picture, and what would a more balanced geographic mix look like?

**Customer understanding**
- Who is the typical customer in terms of age and income - and does that profile match the product mix?
- Is there a demographic segment that is structurally under-served relative to its size in the Brazilian population?
- Does income level correlate with purchase behaviour, or is the base more democratic than expected?

---

## Key Findings

| Finding | Data | Commercial implication |
|---|---|---|
| Revenue concentration | Top 4 departments = 84% of revenue | High supply chain risk - disruption in Phones or Appliances directly impacts monthly results |
| Channel AOV gap | Internet R$974 vs Mobile R$821 (+19%) | Reallocating acquisition budget from Mobile to Internet increases revenue without increasing transaction volume |
| Geographic concentration | SP + RJ + MG = 73% of sales | South, North and Northeast represent structural growth opportunity - low penetration, not low demand |
| Free shipping absorption | R$280k on R$72.6M = 0.39% impact | Policy is commercially viable but should be audited for low-AOV categories where margin compression is highest |
| Senior customer base | 75+ is the largest age bracket (5,096 customers) | UX, support and communication strategy should prioritise clarity and trust over trend-driven design |
| Uniform income distribution | ~4,900 customers per income bracket | Pricing strategy can serve all segments - no need to optimise exclusively for a single income tier |

---

## Dashboard

Three-page interactive report with live filters (channel, card brand, state):

**Executive Overview** - revenue KPIs, daily transaction volume, department breakdown with percentage share, business callouts with commercial interpretation

**Market & Channels** - geographic distribution by state, channel-level performance with AOV comparison, card brand split, transaction volume by department

**Customer Profile** - age distribution, monthly income brackets, geographic origin of customer base, strategic profile summary

---

## Dataset

Two source tables joined on `cliente_Log`:

| Table | Rows | Key fields |
|---|---|---|
| base compra | 80,228 | date, price, freight price, department, state, channel, card brand, customer ID |
| Base cliente | 26,425 | age, income, state of birth, customer ID |

**Period:** 30 March - 13 April 2021  
**Total revenue:** R$72,616,659 (excl. freight) · R$72,896,751 (incl. freight)  
**Unique customers:** 17,040 active in the period

---

## Tech stack

- **HTML / CSS / JavaScript** - zero dependencies, no build step required
- **Chart.js 4.4** - all chart types (line, bar, doughnut)
- **Google Fonts** - Outfit + JetBrains Mono
- **Vercel** - hosting with automatic deploy on push

---


## Project Files

| File | Description |
|---|---|
| `index.html` | Interactive dashboard - open directly in any browser, no setup required |
| `Base_de_dados_desafio_1_2.xlsx` | Source dataset - two sheets: `base compra` (80,228 transactions) and `Base cliente` (26,425 customers) |
| `Desafio_1_Final.pbix` | Original Power BI file with the same analysis built natively in Power BI Desktop |
| `README.md` | This file |

## Run locally

```bash
# No setup required - open directly in browser
open index.html
```

---

## About

Built by **Ingrid Martinez** - Data Analyst with 7+ years in B2B commercial roles at Unilever, Gerdau and Cobli. This project draws on first-hand experience with revenue concentration risk, channel strategy and customer segmentation decisions in large commercial operations.

[LinkedIn](https://www.linkedin.com/in/ingridmartinezm/) · [GitHub](https://github.com/martinez-ie) · [Portfolio](https://ingrid-martinez-portfolio.vercel.app/)
