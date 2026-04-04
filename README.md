# WA-housing-dashboard
A dashbboard to have a quick look for currents housing markets trends in WA.
[README.md](https://github.com/user-attachments/files/26478180/README.md)
# 🏡 WA Housing Research Insights Dashboard

> An interactive, research-grade property market dashboard for Perth & Western Australia — built as a portfolio piece for a Research Analyst role at **[Urbis](https://www.urbis.com.au/)**.

**🌐 Live Dashboard → [adwaitr27.github.io/WA-housing-dashboard](https://adwaitr27.github.io/WA-housing-dashboard/)**

---

![Dashboard Preview](https://images.unsplash.com/photo-1560518883-ce09059eeffa?w=1200&q=80)

---

## 📌 Overview

This single-page decision-support tool translates Perth property market signals into **site strategy, suburb selection, and affordability stories** — structured around the questions a planning and property consultancy answers for its clients every day.

It was built end-to-end in 48 hours as a demonstration of research, analysis, and data storytelling capability — from raw data sourcing through to a fully deployed, interactive dashboard.

---

## 🗂️ What's Inside

| Section | Description |
|---------|-------------|
| **01 — Market Overview** | Demand vs. supply pressure story with key market indicators |
| **02 — Signal Interpretation** | Quick-read table translating data signals into market meaning |
| **03 — Suburb Decision Map** | Interactive bubble chart with 5 client-lens filters |
| **04 — Ranked Shortlist** | Top suburbs scored by client objective |
| **05 — Site Strategy Explorer** | *"What can I do with this land?"* — first-pass advisory tool |
| **06 — Affordability & Rental Stress** | Mortgage repayment ratios and rental stress by income band |
| **07 — Macro Drivers** | RBA rates, interstate migration, building approvals overlay |
| **08 — Market Scenario Explorer** | 3-scenario model: Soft Landing / Prolonged Squeeze / Demand Shock |

---

## 📊 Research Notes

The dashboard is accompanied by a full research package on Notion:

| Document | Link |
|----------|------|
| 📋 Full Research Report | [View on Notion](https://www.notion.so/337efa52acd881918ec0d359106bd837) |
| 🔧 How I Built This Dashboard | [View on Notion](https://www.notion.so/337efa52acd881089d50f3ea8875a39c) |
| 🗃️ Data Sources & Download Guide | [View on Notion](https://www.notion.so/338efa52acd881e2afece09067743529) |

The research report covers:
- Consultant-level interpretation of each chart
- **What Should a Client Do?** — decision framework by stakeholder type (Developer, Government, Investor, First Home Buyer)
- **Market Scenario Explorer** — 24-month forward scenarios with probability weightings and implications per client type

---

## 🔧 Tech Stack

| Layer | Tools |
|-------|-------|
| **Data Collection** | Microsoft Excel (CSV imports from ABS, REIWA, RBA) |
| **Data Wrangling** | Excel (Power Query, XLOOKUP, pivot tables) |
| **Analysis & Modelling** | Excel (scenario modelling, affordability calculators, yield sensitivity tables) |
| **Visualisation** | Vanilla JS + SVG, chart rendering in HTML/CSS |
| **Deployment** | GitHub Pages via GitHub Actions (auto-deploys on push to `main`) |

---

## 📁 Data Sources

All data is sourced from official Australian government and industry sources:

| Dataset | Source | Frequency |
|---------|--------|-----------|
| Median house prices & vacancy | [REIWA](https://reiwa.com.au/the-wa-market/market-data/) | Monthly |
| Building approvals | [ABS Cat. 8731.0](https://www.abs.gov.au/statistics/industry/building-and-construction/building-approvals-australia/latest-release) | Monthly |
| Population & migration | [ABS Cat. 3101.0](https://www.abs.gov.au/statistics/people/population/national-state-and-territory-population/latest-release) | Quarterly |
| Cash rate & mortgage rates | [RBA](https://www.rba.gov.au/statistics/cash-rate/) | Monthly |
| Household income | [ABS Census](https://www.abs.gov.au/census) | Census years |
| Rental yields | [CoreLogic](https://www.corelogic.com.au/news-research/reports/home-value-index) / Calculated | Monthly |
| Land release & zoning | [WAPC](https://www.dplh.wa.gov.au/about/what-we-do/research-and-information/land-supply-monitoring) | Annual |

See the full **[Data Sources & Download Guide](https://www.notion.so/338efa52acd881e2afece09067743529)** for exact file names, Excel prep steps, and a master workbook structure.

---

## 🚀 Deployment

This repo uses **GitHub Actions** to automatically deploy to GitHub Pages on every push to `main`.

```
wa-housing-dashboard/
├── index.html                  ← Full dashboard (single file)
├── README.md                   ← This file
└── .github/
    └── workflows/
        └── deploy.yml          ← GitHub Actions workflow
```

To update the dashboard:
1. Edit `index.html`
2. Commit and push to `main`
3. GitHub Actions redeploys automatically in ~60 seconds ✅

---

## 💡 Key Findings

- Perth median house price has risen **~68% since 2020**, outpacing Sydney and Melbourne
- Rental vacancy rate at **~0.7%** — critically undersupplied, driving 15–20% YoY rent growth
- Building approvals remain **25–30% below the 10-year average**, widening the structural deficit
- WA added an estimated **70,000+ residents in FY2024**, driven by interstate and international migration
- Perth gross rental yields at **4.8–6.0%** are the highest of any Australian capital city

---

## 🔮 What's Next (v2 Roadmap)

- [ ] Live data connections via REIWA API or CoreLogic feed
- [ ] Geospatial suburb map using Leaflet.js / Mapbox
- [ ] Automated weekly data refresh via Python scheduled jobs
- [ ] Forecasting module (ARIMA / Prophet) for 12-month price projections
- [ ] PDF export for client report distribution
- [ ] PowerBI / Tableau version using the same Excel source data

---

## 👤 About

Built by **Adwait Reddy** — Data Analyst & Data Science Graduate, Perth WA.

- 🌐 [Live Dashboard](https://adwaitr27.github.io/WA-housing-dashboard/)
- 📋 [Research Report](https://www.notion.so/337efa52acd881918ec0d359106bd837)
- 💼 Built as a portfolio piece for a Research Analyst role at [Urbis](https://www.urbis.com.au/)

---

*Created: April 2026 · Perth, Western Australia*
