# ☕ Coffee Shop Sales Dashboard

An Excel dashboard I built from scratch analyzing ~10,000 coffee shop transactions across 5 U.S. cities. No Power BI. No Tableau. Just a `.xlsm` file and a whole lot of patience.

---

## Why Excel?

Honestly? I wanted to go back to the basics.

It's so easy to take tools like Power BI and Tableau for granted. You drag a field here, drop a measure there, and boom, you've got a polished dashboard in minutes. But when you strip all of that away and sit in front of a raw Excel workbook, you quickly realize how much those tools are doing for you behind the scenes.

This project humbled me. Every pivot table had to be manually set up. Every chart was formatted by hand. Every slicer connection was wired one by one. Things that take seconds in Tableau took me way longer in Excel, and that's kind of the whole point.

Working in Excel forced me to actually *sit with the data*. There's no "auto-detect relationships." No smart formatting that just figures it out. You're building everything yourself, cell by cell, formula by formula. You're debugging `GETPIVOTDATA` references, fighting with axis labels, trying to get slicers to not look ugly and actually match the colors and feel of the rest of your dashboard, and Googling why your conditional formatting broke for the third time.

It was frustrating. It was slow. And I learned more doing it than I expected.

---

## What the Dashboard Covers

The dataset has **9,971 transactions** from coffee shops in **Austin, Chicago, Los Angeles, New York, and Seattle**, spanning 2021 to 2023.

Here's the high-level picture:

| | |
|---|---|
| Revenue | $46,374 |
| Profit | $16,231 (35% margin) |
| Items Sold | 14,117 |
| Categories | 7 (coffee, cold drinks, desserts, sandwiches, snacks, specialty drinks, tea) |

Chicago brought in the most revenue ($11.2k), followed by LA and New York. Seattle came in last at $5.6k but hey, quality over quantity, right?

Fridays were the busiest day across the board. Desserts were the most profitable category. And revenue stayed surprisingly consistent year over year, hovering around $15k each year with no dramatic swings.

---

## What's Inside the File

```
CoffeeShopSalesDashboard.xlsm
│
├── Dashboard  →  The interactive dashboard with charts and slicers
├── Pivot      →  All the pivot tables feeding the visuals
└── Data       →  Raw data — 9,971 rows, 14 columns
```

The data includes transaction IDs, dates, cities, branches, shop names, product categories, unit prices, quantities, revenue, profit margins, and calculated fields for year, month, and weekday.

17 different shops across 9 branches. Places like Beanery, Loop Latte Lounge, Magnificent Mile Cafe, Sip & Savor, you get the idea.

---

## Tools & Techniques

Nothing fancy here. That was the point.

- **Pivot Tables** for slicing the data every which way (by city, category, year, month, weekday)
- **Formulas** like `SUMIFS`, `GETPIVOTDATA`, `TEXT`, `YEAR`, `WEEKDAY`, and `IFERROR`
- **Charts** like bar, donut, and line, all manually formatted to look cohesive
- **Slicers** wired across multiple pivots for interactive filtering
- **Macros** hence the `.xlsm` format

---

## How to Open It

1. Download the `.xlsm` file
2. Open it in Excel (desktop version works best)
3. Enable macros when prompted
4. Head to the **Dashboard** tab and play around with the slicers

---

*Built with Excel, stubbornness, and way too much coffee.* ☕
