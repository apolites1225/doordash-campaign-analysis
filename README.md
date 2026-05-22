# iFood Marketing Campaign Analysis
**Excel-based customer segmentation and campaign performance study**

![Dashboard Preview](dashboard_preview2.png)

---

## Project Overview

This project analyzes marketing campaign performance across a dataset of 2,021 iFood customers. The goal was to identify which customer segments respond best to campaigns, what drives total spend, and how future campaigns should be targeted for maximum impact.

**Tools used:** Microsoft Excel (Power Query, Power Pivot, DAX, VBA, PivotTables, Slicers, Charts, Conditional Formatting)

---

## The Business Questions

- Which of the 6 campaigns performed best, and why?
- What customer profile is most likely to accept a campaign?
- What drives total customer spend?
- How should future campaigns be targeted?

---

## Dashboard

The interactive dashboard includes:

| Component | Description |
|---|---|
| **KPI 1** | Total Customers |
| **KPI 2** | Acceptance Rate |
| **KPI 3** | Average Spend (all customers) |
| **KPI 4** | Acceptor Avg Spend (campaign acceptors only) |
| **KPI 5** | Top Campaign Rate |
| **Chart 1** | Acceptance Rate by Campaign |
| **Chart 2** | Average Spend by Category |
| **Slicers** | Filter by Income Group, Age Group, Children at Home, Education |

All KPIs and charts update dynamically based on slicer selection.

---

## Workbook Structure

| Sheet | Purpose |
|---|---|
| `Main` | Cleaned dataset — 2,021 rows, 38 columns including demographics, spend by category, channel usage, and campaign responses |
| `Accepted Customer Profile` | PivotTable summarizing spend profile and acceptance rates for customers who accepted each campaign |
| `Calculations` | Named cells powering KPI cards on the dashboard |
| `Dashboard` | Interactive visual layer with charts, KPIs, and slicers |

---

## Key Findings

**1. Campaign 6 was the clear winner**
Campaign 6 achieved a 15.4% acceptance rate — more than double the next best campaign (7.7%). The overall average across all campaigns was 7.6%.

**2. Campaign acceptors spend significantly more**
Customers who accepted any campaign averaged $932 in total spend vs. $564 for all customers — a 65% difference.

**3. Income is the strongest spend driver**
The $75K+ income group (16% of customers) averaged $1,373 in total spend — nearly double the $50K–$75K group ($783) and 25x the sub-$25K group ($54).

**4. $75K+ customers are the most campaign-responsive**
This segment accepted Campaign 5 at 37.6% — the highest rate of any income/campaign combination. Campaign 6 was the top performer across all other income groups at 11–12%.

**5. Children at home significantly reduce spend**
Households with no children averaged $846 in total spend vs. $183 for those with one child and $107 for those with two.

**6. Wine and meat dominate the product mix**
Wines represent 54.4% of average spend ($306), meat products 29.5% ($166). Together they account for 83.9% of all customer spending.

**7. Campaign 2 significantly underperformed**
At 1.3% acceptance (26 customers), Campaign 2 was nearly an order of magnitude less effective than Campaign 6.

---

## Data & Methodology

**Dataset:** 2,021 customer records (after deduplication) with the following variable groups:
- **Demographics:** Age, income, marital status, education, household composition
- **Spend:** Total spend + breakdown across 6 product categories (wines, fruits, meat, fish, sweets, gold)
- **Channels:** Web, catalog, and in-store purchase counts; web visits per month
- **Campaigns:** Binary acceptance flags for Campaigns 1–6
- **Engagement:** Days since last purchase (recency), days as a customer, complaint flag

**Excel techniques applied:**
- Power Query for data transformation, cleaning, and deduplication
- Power Pivot for data modeling with unpivoted campaign structure
- DAX measures using AVERAGEX and DISTINCTCOUNT to correctly calculate per-customer averages across unpivoted data
- VBA for automated filter reset functionality
- Slicers connected to multiple PivotTables for cross-filtering
- Conditional formatting to highlight performance outliers

---

## How to Use

1. Download `iFood_campaign_analysis.xlsm`
2. Enable macros if prompted
3. Navigate to the **Dashboard** tab
4. Use the slicers to filter by Income Group, Age Group, Children at Home, or Education
5. All KPIs and charts update dynamically based on slicer selection
6. Click **Reset Filters** to return to the full dataset view

---

## Business Recommendations

| Priority | Recommendation |
|---|---|
| 🎯 Target | $75K+ income, child-free customers for premium campaigns |
| 📦 Lead with | Wine and meat — they represent 84% of wallet share |
| 📈 Scale | Campaign 6's structure for volume (15.4% acceptance); Campaign 5's for high-LTV $75K+ targeting (37.6%) |
| ❌ Retire | Campaign 2's approach — 1.3% acceptance is not scalable |
| 👴 Don't ignore | 66+ age group — highest avg spend ($699) and campaign acceptance (30%) |

---

## About

This case study was completed as part of a self-directed data analytics portfolio.
Feel free to connect on [LinkedIn](https://linkedin.com/in/aristotlepolites/) if you have questions or feedback.
