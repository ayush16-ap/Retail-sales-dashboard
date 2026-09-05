# Retail Sales Dashboard

A Power BI dashboard for analyzing retail sales across products, customers, and regions. Built on a star schema data model with 5 report pages covering sales trends, regional performance, profitability, and root-cause analysis.

## Data Model

Star schema with one fact table and three dimension tables:

```
Dim_Products ──┐
Dim_Customers ─┼── Fact_Sales
Dim_Date ──────┘
```

- `Fact_Sales` — Total Sales, Quantity, Profit, region-wise sales
- `Dim_Products` — product name, category, unit price
- `Dim_Customers` — customer name, region
- `Dim_Date` — Year → Quarter → Month → Day hierarchy

## Report Pages

| Page | Content | Visuals |
|---|---|---|
| 1. Sales Overview | Product and monthly sales trends | Column chart, line chart, pie chart, table |
| 2. Regional & Customer Analysis | Sales by region and customer | Bar chart, funnel, waterfall, pivot table, slicers |
| 3. Category & Profit Insights | Category contribution, top/bottom performers | Donut chart, treemap, KPI, gauge, pivot table |
| 4. Root Cause Analysis | Drivers behind total sales | Decomposition tree, key influencers |
| 5. Trend Analysis | Sales trend vs. quantity sold | Line chart, scatter chart |

## Tech Stack

- Power BI Desktop
- DAX (measures for sales, profit, regional splits)
- Star schema data modeling

## Setup

```bash
git clone https://github.com/ayush16-ap/Retail-sales-dashboard.git
```

Open the `.pbix` file in Power BI Desktop. Use the slicers and navigation buttons to filter by region, product, category, and date. On Page 4, use the decomposition tree to drill into what's driving total sales.

## Author

Ayush — BTech Mining Engineering, IIT (ISM) Dhanbad
