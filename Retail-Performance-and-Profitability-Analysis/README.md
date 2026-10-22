# Retail Performance & Profitability Analysis

## Project Overview

This project analyzes retail sales and profitability using Microsoft Power BI and the Sample Superstore dataset. The interactive dashboard provides insights into sales trends, regional performance, customer segments, product profitability, and discount patterns to support data-driven business decisions.

## Objectives

- Evaluate overall sales, profit, order volume, and profit margin.
- Analyze monthly sales and profit trends.
- Compare sales performance across product categories and customer segments.
- Identify regional and product sub-categories with strong or weak profitability.
- Explore the relationship between discounts and product profitability.

## Tools & Technologies

- **Power BI Desktop** — Dashboard development and data visualization
- **Power Query** — Data inspection and transformation
- **DAX** — Measure creation and KPI calculations
- **CSV** — Dataset format

## Dashboard Pages

### 1. Retail Performance Overview

Provides a high-level view of business performance, including:

- Key performance indicators: Total Sales, Total Profit, Total Orders, and Profit Margin
- Monthly sales and profit trends
- Sales by product category
- Profit by region
- Sales by customer segment
- Interactive filters for order date, region, and segment

### 2. Product & Profitability Analysis

Examines product-level performance through:

- Profit by sub-category
- Sales versus profit by product
- Discount versus profit by product
- Product-level sales, profit, and profit margin table

## Key Findings

- **Total Sales:** Approximately 2.30 million
- **Total Profit:** Approximately 286.40K
- **Overall Profit Margin:** 12.47%
- **Category Performance:** Technology recorded the highest sales among the three categories.
- **Regional Performance:** The West region generated the highest total profit.
- **Customer Segments:** The Consumer segment contributed approximately 50.56% of total sales.
- **Product Profitability:** Copiers and Phones were among the strongest profit contributors by sub-category, while Tables recorded a substantial loss.
- **Discount Analysis:** Profitability varied across discount levels, with several products exhibiting significant losses.

These findings are based on the current dashboard aggregations. Observed relationships between discounts and profit do not establish causation.

## DAX Measures

```dax
Total Sales = SUM('DataSet'[Sales])

Total Profit = SUM('DataSet'[Profit])

Total Orders = DISTINCTCOUNT('DataSet'[Order ID])

Profit Margin = DIVIDE([Total Profit], [Total Sales], 0)
```

## Project Structure

```text
Retail-Performance-and-Profitability-Analysis/
├── Datasets/
│   └── DataSet.csv
├── PowerBI/
│   └── Retail_Performance_Analysis.pbix
├── Screenshots/
│   ├── 01_Retail_Performance_Overview.png
│   └── 02_Product_Profitability_Analysis.png
└── README.md
```

## Skills Demonstrated

- Data preparation and type transformation
- DAX measures and KPI development
- Interactive dashboard design
- Data visualization and exploratory analysis
- Sales and profitability analysis
- Business insight generation

## Future Enhancements

- Year-over-year performance analysis
- Shipping and delivery performance analysis
- Deeper investigation of discounting and profitability
- Additional DAX measures and drill-through functionality

## Dataset

**Dataset:** Sample Superstore

**Source:** Add the original dataset download URL before publishing the repository.

The dataset's source and licence should be verified before redistributing the file.

## Author

**Nazreen Shanavaz**


