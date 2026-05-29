# Dataset

This folder contains the source dataset used in this project.

## File

```text
sample_-_superstore.xls
```

## Source

Dataset: [**Superstore Dataset by Divy Jain**](https://www.kaggle.com/datasets/divyjain28/superstore-sales)
Platform: **Kaggle**

## Description

The dataset contains Superstore sales transaction records. It includes order information, customer details, product categories, sales amount, quantity, discount, and profit.

Key columns include:

- Row ID
- Order ID
- Order Date
- Ship Date
- Ship Mode
- Customer ID
- Customer Name
- Segment
- Country
- City
- State
- Postal Code
- Region
- Product ID
- Category
- Sub-Category
- Product Name
- Sales
- Quantity
- Discount
- Profit

## How This Dataset Is Used

The notebook uses this dataset to build an automated revenue and profit monitoring workflow.

Main steps:

1. Load the source Excel file
2. Inspect columns, data types, and missing values
3. Convert date columns into proper datetime format
4. Create reporting fields such as year, month, month-year, and shipping days
5. Split the dataset into monthly CSV files
6. Combine monthly files automatically
7. Validate data quality
8. Calculate business KPIs
9. Detect revenue and profit risk areas
10. Generate charts and final output reports

## Project Outputs Created From This Dataset

The dataset is used to generate:

- Monthly KPI summary
- Data validation summary
- Business risk alerts
- Category-level risk summary
- Region-level risk summary
- Risky months report
- Business insights report
- Revenue and profit visualizations

## Note

This dataset is used for educational and portfolio purposes. Please refer to the original Kaggle dataset page for ownership, license, and usage terms.
