# Retail Sales Overview Dashboard | Power BI

## Project Overview

This project presents a Power BI dashboard exploring a fictional retail sales dataset for January–June 2026. It demonstrates a beginner data-analysis workflow: preparing sales data, calculating revenue and profit, and using visuals to compare performance over time, across product categories, by product, and by city.

> **Data disclaimer:** This project uses synthetic practice data. It does not represent a real company, real customers, or actual commercial performance.

## Business Questions

The dashboard is designed to explore four questions:

1. How does revenue change from month to month?
2. Which product categories contribute the most revenue?
3. How is revenue distributed across individual products?
4. How does profit compare across cities?

## Dashboard Preview

Add a screenshot of your actual Power BI report at `screenshots/dashboard.png` and uncomment the image below.

<!-- ![Retail Sales Overview dashboard](screenshots/dashboard.png) -->

## Dashboard Visuals

| Visual | Fields / measure | Purpose |
|---|---|---|
| Revenue by Category | `Category` and `Revenue` (Sum) | Compare revenue across product categories |
| Revenue Share by Product | `Product` and `Revenue` (Sum), donut chart | Explore each product's share of revenue |
| Monthly Revenue Trend | `OrderDate` (Year and Month) and `Revenue` (Sum), area chart | Review how revenue changes over time |
| Profit by City | `City` and `Profit` (Sum) | Compare profit across cities |

The visuals are intended to support exploration of the sample data. Add specific conclusions only after checking the values shown in Power BI.

## Tools Used

- **Microsoft Power BI Desktop** — report and dashboard visuals
- **Power Query** — data preparation and calculated columns
- **CSV** — source data
- **GitHub** — project documentation and portfolio sharing

## Dataset

The source file is `data/retail_sales.csv`. It contains 24 synthetic sales-line records dated January through June 2026.

| Field | Description |
|---|---|
| `OrderDate` | Date of the sales line |
| `City` | City associated with the sale |
| `Category` | Product category |
| `Product` | Product name |
| `UnitPriceEUR` | Selling price per unit in euros |
| `UnitCostEUR` | Cost per unit in euros |
| `Quantity` | Number of units sold |

Each row represents a sales line, not necessarily a unique customer order.

## Data Preparation and Calculations

The report uses the following row-level calculations:

- **Revenue** = `UnitPriceEUR × Quantity`
- **TotalCost** = `UnitCostEUR × Quantity`
- **Profit** = `Revenue − TotalCost`

These columns allow Power BI to sum the measures across categories, products, dates, and cities. The calculated values should be checked against the source data before drawing conclusions.

## How to Open the Project

1. Download or clone this repository.
2. Open `Retail_Sales_Overview_Jan-Jun_2026.pbix` in Power BI Desktop.
3. If Power BI asks for the source file, select `data/retail_sales.csv` and refresh the data.
4. Review the report page and interact with the visuals.

## Key Findings

Complete this section after reviewing the actual report. Do not leave unsupported example claims in the published version.

- **Highest-revenue category:** [Add the category and value shown in Power BI]
- **Largest product revenue contribution:** [Add product and value]
- **Highest-profit city:** [Add city and value]
- **Revenue trend:** [Describe the trend across January–June 2026]

## Limitations

- The dataset is small and synthetic, so it cannot support conclusions about a real retailer.
- The reporting period covers only six months.
- The data is designed for learning and dashboard demonstration, not real business decisions.
- Revenue and profit calculations depend on correct source values and data types.

## Possible Future Improvements

- Add KPI cards for total revenue, total profit, profit margin, and units sold.
- Add slicers for city, category, and date.
- Improve date handling and add a dedicated calendar table.
- Add a short, evidence-based interpretation of the results.
- Expand the dataset and test the report with more records.

## Author

Created as a learning project to develop practical data analysis and Power BI skills.
