# 🛒 Woolworths Everyday Rewards – Loyalty KPI Dashboard

<img width="1102" height="618" alt="Screenshot 2026-04-13 111114" src="https://github.com/user-attachments/assets/0b229b55-5cce-4424-92ca-1fb182099154" />


## 📌 Overview

This Power BI project was developed as part of a data analytics case study simulating 
the role of a Data Analyst at Woolworths. The goal was to build an interactive dashboard 
for the sales team to monitor the performance of the **Everyday Rewards** loyalty program 
across Sydney stores, enabling data-driven decision-making.

---

## 📊 Dashboards

### 1. Woolworths Loyalty KPI Dashboard
The main overview dashboard providing a high-level summary of loyalty program performance.

**KPI Cards:**
- No. of Customers Registered (CY23)
- No. of Transactions (until EOFY 2024)
- Total Points Earned (Everyday Rewards)
- Total Points Redeemed (Everyday Rewards)
- Total Transaction Amount (AUD)

**Visuals Included:**
| Visual | Description |
|--------|-------------|
| Customer Registration Trend | Line chart showing monthly registration trends with a trendline |
| Points by Time | Dual-axis line chart for Points Earned vs Redeemed over time |
| Top 5 Store Locations by Points Earned | Treemap of highest-performing Sydney stores |
| Points Redeemed by Redemption Type | Donut chart (Shopping Discount, Fuel Discount, Donation) |
| Customer Membership Status | Donut chart showing Active vs Suspended vs Inactive members |
| Top 10 Redeemers | Horizontal bar chart of highest points redeemers |
| Points Earned vs Redeemed by Store | Scatter plot comparing store-level earn/redeem behaviour |

**Filter:** Year slicer (2023 / 2024)

---


<img width="1103" height="606" alt="Screenshot 2026-04-13 111130" src="https://github.com/user-attachments/assets/76785257-33ff-4734-82dc-790e290110b8" />

### 2. Drill-Through Report – Store Location Deep Dive
A context-sensitive drill-through page that activates when a store is selected on the 
main dashboard, providing granular store-level insights.

**KPI Cards (Store-Specific):**
- % of Redeemed Points
- % Contribution to Total Points Earned
- % Contribution to Total Points Redeemed
- Threshold Redemption %

**Visuals Included:**
| Visual | Description |
|--------|-------------|
| Top 10 Point Earners | Bar chart of customers with highest points earned at the store |
| Top 10 Point Redeemers | Bar chart of customers with highest redemptions |
| Points Earned & Redeemed Over Time | Dual-axis line chart for store-level trend |
| Relation Between Points Earned & Redeemed | Scatter plot with trendline |
| Dynamic Insight Card | Auto-generated text summarising key insights for the selected store |

---

## ⚙️ Technical Implementation

### DAX Measures
Custom DAX formulas were written for:
- `% of Points Redeemed` = Points Redeemed / Points Earned
- `% Contribution to Total` = Store Points / All Stores Points
- Running totals, rankings, and dynamic text for the insight card

### Quick Measures Used
- Year-over-year comparisons
- Percentage of total calculations
- Top N customer rankings

### Data Model
- Star schema with a central fact table (transactions) linked to dimension tables 
  (customers, stores, dates, redemption types)
- Relationships established across all tables for cross-filtering

---

## 🗂️ Files

| File | Description |
|------|-------------|
| `Woolworths_Dashboard.pbix` | Main Power BI file |
| `dataset/` | Raw data files used in the project |
| `preview.png` | Dashboard screenshot |

---

## 🔗 Links
- 📁 https://www.datascienceportfol.io/shahneel364/projects/5
- 💻 [GitHub Repository](https://github.com/neel244)

---

## 🏷️ Skills Used
`Power BI` `DAX` `Data Visualisation` `Drill-Through Reports` `Quick Measures` 
`Data Modelling` `KPI Analysis` `Business Intelligence` `Retail Analytics`
