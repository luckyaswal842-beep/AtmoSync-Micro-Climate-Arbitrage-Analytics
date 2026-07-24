# 🥑 AtmoSync — Micro-Climate Arbitrage Analytics

**Team Members:**
* Lucky Aswal
* Mameeth C
* Aparna C
* Malavika Nair

**Infotact Data Analytics Project | Progress & Status Report**

> Real-time IoT sensor analytics to detect in-transit commodity spoilage and identify profitable reroute ("arbitrage") opportunities before goods degrade below quality thresholds.

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458)
![Status](https://img.shields.io/badge/Status-Week%202%20Complete-brightgreen)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📌 Project Overview

Traditional supply chain analytics rely on standard transit times and macro-weather forecasts — they miss hyper-local micro-climate shifts (e.g. a humidity spike inside one specific container) that quietly spoil agricultural cargo before it reaches market.

**AtmoSync** simulates a live IoT sensor pipeline for refrigerated shipping containers, calculates a real-time **spoilage risk score**, and flags **"Spoilage Arbitrage"** opportunities — cases where rerouting a container to a closer secondary market preserves more value than pushing on to the original destination.

This repository documents our work as the **Data Analytics Team** on the project, using Python, pandas, data visualizations, and executive presentation materials to build actionable business insights.

---

## ✅ Progress Tracking

### Week 1 — Data Foundations & EDA
| # | Task | Status |
|---|------|--------|
| 1 | Defined dataset schema (sensor, logistics, and pricing fields) | ✅ Done |
| 2 | Generated 50,000-row synthetic IoT dataset (550 containers × ~91 readings) | ✅ Done |
| 3 | Performed 9-step data cleaning process & business-rule validation | ✅ Done |
| 4 | Conducted initial Exploratory Data Analysis (EDA) on spoilage factors | ✅ Done |
| 5 | Compiled findings into stakeholder-ready reports | ✅ Done |

### Week 2 — Dashboard Visualizations & In-Depth Modeling
| # | Task | Status |
|---|------|--------|
| 1 | Generated baseline temperature tracking & anomaly distribution visuals | ✅ Done |
| 2 | Modeled quality degradation across specific commodities and transit hours | ✅ Done |
| 3 | Mapped risk status severity against automated action workflows | ✅ Done |
| 4 | Evaluated multi-metric correlation matrix for micro-climate factors | ✅ Done |
| 5 | Performed market price comparisons for micro-climate arbitrage | ✅ Done |

---

## 📊 Key Findings & Visual Insights (Week 2)

### 1. Temperature Control & Drift Tracking
* **Trace Analysis (`chart1_temperature_trace.png`):** Real-time monitoring shows distinct containers exceeding safe thermal limits during mid-transit.
* **Deviation Distribution (`chart2_temp_deviation_hist.png`):** Temperature variance strongly skews right, confirming that localized cooling unit failures cause severe thermal spikes.

### 2. Commodity Spoilage & Quality Modeling
* **Quality by Commodity (`chart3_quality_by_commodity.png`):** High-sensitivity commodities (Strawberries, Blueberries) exhibit significantly sharper quality loss when exposed to thermal shifts compared to hardier cargo like Tomatoes.
* **Transit Duration vs. Quality (`chart4_quality_vs_transit_scatter.png`):** Demonstrates a direct inverse correlation between total transit hours and container quality retention, accelerating rapidly after temperature breach events.

### 3. Risk Assessment & Arbitrage Potential
* **Risk & Action Distribution (`chart5_risk_and_action_counts.png`):** Categorizes fleet status across *Normal*, *Watch*, *At-Risk*, and *Critical* states to trigger automated rerouting actions.
* **Metric Correlations (`chart6_correlation_heatmap.png`):** Reaffirms that `temp_deviation_c` holds the strongest negative correlation ($r = -0.84$) with `quality_score`.
* **Price Arbitrage Comparison (`chart7_price_comparison.png`):** Highlights market price differentials between primary and secondary ports, supporting real-time rerouting decisions to maximize recovered value.

---

## 🛠️ Tools Used

| Purpose | Tool |
|---|---|
| Data generation & manipulation | Python, pandas, numpy |
| Data cleaning & validation | pandas |
| Exploratory analysis & statistical modeling | pandas (`groupby`, `corr`, `value_counts`) |
| Visualizations & Dashboards | matplotlib, seaborn |
| Executive Presentation | Microsoft PowerPoint (`AtmoSync.pptx`) |
| Version control | Git & GitHub |

---

## 📁 Repository Structure

```text
atmosync-analytics/
│
├── data/
│   ├── atmosync_dataset.csv              # Raw dataset (50,000 rows)
│   └── cleaned_dataset.csv               # Cleaned & validated dataset
│
├── notebooks/
│   ├── Dataset Cleaning.ipynb            # Initial cleaning & validation workflow
│   └── week2_dashboard_and_insights.ipynb# Visual dashboard & analysis generation
│
├── visuals/
│   ├── chart1_temperature_trace.png       # Continuous temperature monitoring trace
│   ├── chart2_temp_deviation_hist.png     # Distribution of temperature deviations
│   ├── chart3_quality_by_commodity.png    # Quality degradation per produce type
│   ├── chart4_quality_vs_transit_scatter.png # Transit duration vs. quality correlation
│   ├── chart5_risk_and_action_counts.png  # Risk severity vs. action counts
│   ├── chart6_correlation_heatmap.png     # Multi-metric feature correlation map
│   └── chart7_price_comparison.png        # Primary vs. secondary market prices
│
├── AtmoSync.pptx                         # Stakeholder deck
└── README.md

## 👤 Author

**Data Analyst — AtmoSync Project**
GitHub: https://github.com/luckyaswal842-beep


