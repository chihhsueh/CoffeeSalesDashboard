# ☕ Coffee Shop Sales Dashboard — Excel Project

A fully interactive sales dashboard analyzing **9,971 transactions** across **5 U.S. cities**, built entirely in Microsoft Excel. No Power BI. No Tableau. Just `.xlsm`.

---

## 📊 Key Metrics

| Metric | Value |
|--------|-------|
| **Total Revenue** | $46,374.25 |
| **Total Profit** | $16,230.99 |
| **Profit Margin** | 35% |
| **Transactions** | 9,971 |
| **Qty Sold** | 14,117 |
| **Cities** | 5 |
| **Categories** | 7 |
| **Time Span** | 2021 – 2023 |

---

## 💭 Reflection — Back to the Basics

There's a moment when you open a blank Excel workbook — no drag-and-drop visuals, no AI-assisted formatting, no one-click dashboards — and you realize just how much we take tools like **Power BI** and **Tableau** for granted.

This project was a deliberate return to the fundamentals. Every pivot table had to be manually configured. Every chart painstakingly formatted. Every slicer connection hand-wired. What takes three clicks in Tableau can take thirty minutes in Excel — and that's precisely the point.

Going back to the basics forced me to *truly understand the data*. There's no "auto-detect relationships" here. You build the structure yourself, cell by cell, formula by formula. You wrestle with `GETPIVOTDATA`, fight with conditional formatting rules, and learn why your chart axes refuse to cooperate. It's humbling, and it's clarifying.

The result? A fully interactive dashboard tracking revenue, profit margins, and sales trends across 5 cities and 3 years — all within the constraints of a `.xlsm` file. No external connections. No premium licenses. Just Excel.

> *If you know Excel, you can learn anything.*

---

## 📈 Dashboard Breakdown

### Revenue & Profit by Month
Monthly revenue ranges from ~$3,500 to ~$4,500, with January being the strongest month ($4,543.62). Profit tracks consistently at a 35% margin across all months.

### Revenue by Category
| Category | Revenue |
|----------|---------|
| Desserts | $7,204.40 |
| Tea Beverages | $6,674.11 |
| Sandwiches | $6,756.61 |
| Coffee Beverages | $6,534.52 |
| Specialty Drinks | $6,496.38 |
| Snacks | $6,423.38 |
| Cold Drinks | $6,284.85 |

### Revenue by City
| City | Revenue |
|------|---------|
| Chicago | $11,206.32 |
| Los Angeles | $10,787.47 |
| New York | $10,425.45 |
| Austin | $8,367.80 |
| Seattle | $5,587.21 |

### Revenue by Year
| Year | Revenue |
|------|---------|
| 2021 | $15,252.78 |
| 2022 | $15,746.59 |
| 2023 | $15,374.88 |

### Transactions by Weekday
Friday leads with **1,498** transactions. Distribution is relatively even across all days, with Monday being the quietest at 1,390.

### Profit by Category
Desserts lead profitability at **$2,521.54**, while Cold Drinks trail at $2,199.70.

---

## 🛠 Tools & Techniques

- **Pivot Tables** — Multiple pivots slicing data by category, city, year, month, and weekday. The backbone of the entire dashboard.
- **Formulas** — `SUMIFS`, `GETPIVOTDATA`, `TEXT`, `YEAR`, `WEEKDAY`, `IFERROR` — calculated fields for profit margins and time-based dimensions.
- **Excel Charts** — Bar charts, donut charts, and line graphs, each manually formatted for a cohesive visual identity.
- **Slicers** — Connected slicers enabling dynamic filtering across all dashboard components.
- **VBA/Macros** — `.xlsm` format to support macro-enabled interactivity.

---

## 📂 File Structure

```
CoffeeShopSalesDashboard.xlsm
├── Dashboard    — Interactive visual dashboard with slicers
├── Pivot        — Pivot tables powering all visualizations
└── Data         — Raw dataset (9,971 rows × 14 columns)
```

### Data Columns
`Transaction ID` · `Date` · `City` · `Branch` · `Shop Name` · `Product ID` · `Product Category` · `Unit Price` · `Qty Sold` · `Revenue` · `Profit Margin` · `Year` · `Month` · `Weekday`

---

## 🏙 Cities & Locations

| City | Branches |
|------|----------|
| Austin | Zilker Park, Central Park |
| Chicago | Michigan Avenue, Madison Street |
| Los Angeles | Venice Beach, Capitol Hill, Hollywood Hills |
| New York | Brooklyn, Central Park |
| Seattle | Capitol Hill, Pike Place |

**17 unique shops** including Coffee House, Beanery, Espresso, Loop Latte Lounge, Magnificent Mile Cafe, Park Brew, Sip & Savor, and more.

---

## 🚀 How to Use

1. Download `CoffeeShopSalesDashboard.xlsm`
2. Open in Microsoft Excel (desktop version recommended)
3. **Enable macros** when prompted
4. Navigate to the **Dashboard** sheet
5. Use the slicers to filter by city, category, year, etc.

---

*Built with Excel, patience, and a lot of coffee.* ☕
