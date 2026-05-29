# Automated Revenue & Profit Monitoring System

## Project Overview

This project is an automated business reporting workflow built with Python. It processes Superstore sales data, validates data quality, calculates key revenue and profitability KPIs, detects business risks, creates visual reports, and exports stakeholder-ready output files.

The goal of this project is to simulate a real data analyst reporting task where monthly sales files need to be combined, cleaned, analyzed, and converted into useful business insights.

## Business Problem

Sales and operations teams often receive transaction data in separate monthly files. Manually combining these files, checking data quality, calculating KPIs, and preparing reports can be time-consuming and error-prone.

This project solves that problem by creating a repeatable Python workflow that automates the reporting process and highlights areas that require business attention.

## Dataset

Dataset used: **Superstore Dataset by Divy Jain** from Kaggle.

The dataset contains sales transaction records with fields such as:

- Order Date
- Ship Date
- Region
- Category
- Sub-Category
- Product Name
- Sales
- Quantity
- Discount
- Profit

## Tools Used

- Python
- pandas
- matplotlib
- Google Colab

## Project Workflow

1. Load the Superstore dataset
2. Inspect columns, data types, and missing values
3. Convert date columns into proper datetime format
4. Create reporting columns such as year, month, month-year, and shipping days
5. Split the dataset into monthly CSV files to simulate recurring monthly reports
6. Automatically combine monthly CSV files into one reporting dataset
7. Run data validation checks
8. Calculate business KPIs
9. Detect revenue and profit risk areas
10. Create visual charts
11. Export final CSV reports and business insights

## Data Validation Checks

The project includes validation checks for:

- Missing required columns
- Missing values
- Duplicate rows
- Negative sales values
- Zero or negative quantity values
- Invalid discount values
- Ship dates earlier than order dates

These checks help ensure that the reporting output is based on reliable data.

## KPIs Calculated

The project calculates the following KPIs:

- Total Sales
- Total Profit
- Total Orders
- Total Quantity Sold
- Average Order Value
- Profit Margin
- Average Discount
- Monthly Sales Growth
- Monthly Profit Growth

## Business Risk Detection

The project includes rule-based alerts to identify:

- High sales but low profit products
- Loss-making products
- High discount and negative profit products
- Weak category-level profit margins
- Weak region-level profit margins
- Monthly sales drops
- Monthly profit drops
- Monthly margin drops

This makes the project more than a basic sales report. It acts as a simple business performance monitoring system.

## Visualizations

The notebook creates and saves the following charts:

- Monthly Sales Trend
- Monthly Profit Trend
- Profit Margin by Category
- Sales vs Profit by Region
- Top 10 Loss-Making Products

## Output Files

The project exports final reports such as:

- `kpi_summary.csv`
- `monthly_kpi_summary.csv`
- `data_validation_summary.csv`
- `business_risk_alerts.csv`
- `category_risk_summary.csv`
- `region_risk_summary.csv`
- `risky_months.csv`
- `business_insights.txt`

## Key Business Questions Answered

This project helps answer questions such as:

- Which months had the highest and lowest sales?
- Which months had the highest and lowest profit?
- Which products generated losses?
- Which products had high sales but weak profitability?
- Which categories had the weakest profit margins?
- Which regions had weaker profitability?
- Is discounting connected with lower profitability?
- Which months showed performance risk?

## How to Run

1. Open the notebook in Google Colab.
2. Upload the Superstore dataset file.
3. Run the notebook cells from top to bottom.
4. Review generated charts and output reports.

Required libraries:

```text
pandas
matplotlib
xlrd
