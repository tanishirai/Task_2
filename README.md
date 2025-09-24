# Superstore Sales Dashboard - Power BI

## Overview

This project contains a **single-page executive dashboard** developed in Power BI to analyze the Superstore sales data. The dashboard offers actionable insights into sales performance, profitability, customer segmentation, and regional analysis using well-crafted visualizations.

## Included Files

- `Sample - Superstore.csv`: The source dataset containing sales records, customer info, product details, and geography.
- `sales_dashboard.pbix`: The Power BI dashboard file with all data transformations, DAX measures, and visuals.
- `sales_dashboard.pdf`: Exported PDF version of the dashboard for offline viewing.

## Dashboard Features

- **KPI Cards**: Total Sales, Total Orders, Total Customers, Total Profit.
- **Profit by Category**: Bar chart illustrating sales and profit by product category.
- **Profit by Region**: Regional profit distribution across US regions.
- **Sales & Customers by State**: Geographic bubble map visualization.
- **Profit by Customer Segment**: Bar chart showing sales by consumer segments.
- **Average Profit Margin**: Gauge showing overall profitability ratio.
- **Sales and Profit Trend by Month**: Line chart revealing sales and profit trends over time.

## Dataset Preparation and Cleaning

- Used Power Query Editor for data cleaning:
  - Date columns converted to proper date types.
  - Removed nulls and inconsistencies.
  - Added calculated columns: Profit Margin, Days to Ship, Year, Month Name.
- Validated data quality before visualization.

## Calculated Columns & Measures (DAX)

- `Profit Margin = DIVIDE(Profit, Sales, 0)`
- `Days to Ship = DATEDIFF(Order Date, Ship Date, DAY)`
- `Year = YEAR(Order Date)`
- `Month Name = FORMAT(Order Date, "MMMM")`
- Other measures for KPIs and chart data aggregations.

## How to Use

1. Open `sales_dashboard.pbix` in Power BI Desktop.
2. Load or connect to the included `Superstore.csv` data.
3. Interact with slicers and visual filters to explore insights.
4. Export dashboard as PDF or publish to Power BI service as needed.

## Tools and Technologies

- Power BI Desktop (for dashboard creation)
- DAX (for calculations and measures)
- Power Query (for ETL/data cleaning)

## Screenshots

See the `sales_dashboard.pdf` for visual snapshot of the dashboard layout and key charts.

---
