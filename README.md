# Retail Sales Performance Dashboard

## Project Overview

This project is an interactive Power BI dashboard designed to analyse retail sales performance across products, categories, regions and time periods.

The dashboard provides a clear overview of key business metrics and allows users to explore sales performance using interactive filters.

## Key KPIs

- Total Sales: $382.57K
- Total Profit: $172.22K
- Total Orders: 1.2K
- Profit Margin: 45%

## Dashboard Features

- Monthly Sales Trend
- Sales by Region
- Sales by Category
- Top 5 Products by Sales
- Year Filter
- Region Filter

## Tools Used

- Power BI
- Power Query
- DAX
- CSV
- Data Cleaning
- Data Visualisation

## Data Preparation

The dataset was cleaned and transformed in Power Query before building the dashboard.

Key preparation steps included:

- Checking data types
- Removing duplicate Order IDs
- Checking missing values
- Validating numeric columns
- Preparing date fields for monthly trend analysis

## DAX Measure

```DAX
Profit Margin =
DIVIDE(
    SUM(retail_sales_powerbi_dataset[Profit]),
    SUM(retail_sales_powerbi_dataset[Sales]),
    0
)
