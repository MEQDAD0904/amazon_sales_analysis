# Amazon Sales Dashboard (Excel)

An interactive two-page Excel dashboard analyzing ~50K e-commerce orders (2022–2023): an executive overview, then a diagnostic page that asks *why* revenue looks the way it does.

> **Note:** This is a graduation project built on a **synthetic dataset**, so many segments show near-uniform results. Reporting "no meaningful difference" is treated as a valid finding.

## Dataset
- ~50,000 orders with: order date, product category, price, discount %, quantity sold, customer region, payment method, rating, review count, discounted price, and total revenue.
- The `profit` column was excluded because there is no cost data to verify it (it is a flat 5% of revenue).

## Dashboard Pages

### 1. Executive Overview
- KPIs: Total Sales ($32.87M), Total Quantity, Total Orders, Avg Order Value ($657)
- Sales trend by quarter, sales by category, sales by region, payment distribution
- Slicers: payment method, product category, region

### 2. Diagnostic Analysis
- KPIs: Avg Discount (13%), Avg Price ($253), Avg Review (3.0), Lost Revenue to Discounts ($5.05M)
- Avg order revenue & avg quantity by discount level
- Revenue by price band (Low <150, Mid 150–300, High >300)
- Avg order revenue by rating
- Key Insights card

## Key Findings
- **Price drives revenue:** High-price orders (>$300) generate $21.09M, about 64% of total revenue.
- **Discounts don't lift volume:** avg order revenue falls from $749 (0% discount) to $522 (30%), while avg quantity stays at 3.0 and order counts are even across levels (~8.2K–8.5K).
- **Ratings show no effect:** avg order revenue stays within $640–$665 across rating bands.
- **No dominant segment:** category and region revenues are nearly identical (~$1.3M–$1.4M each).

## Tools & Techniques
- Microsoft Excel: Pivot Tables, PivotCharts, Slicers (shared across pivots), helper columns (`price_band`, `revenue_before_discount`), GETPIVOTDATA-linked KPI cards, combo charts
- Data cleaning and dashboard design

## Files
- `Final Project.xlsx`: the full workbook (data, pivots, dashboard pages)
- `/screenshots`: dashboard previews

## Author
[Your Name] | [LinkedIn link]
