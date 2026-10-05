# Online Retail Data Cleaning & Preparation

## Project Overview

This project focuses on cleaning and preparing an Online Retail
transaction dataset for further exploratory data analysis and
business intelligence reporting.

The dataset contains information about invoices, products,
quantities, prices, customers and countries.

## Dataset

The original dataset was obtained from Kaggle and provided as a CSV
file.

The original dataset contained 8 columns. During the cleaning and
preparation process, a Revenue column was created.

## Tools Used

- Microsoft Excel
- Power Query

## Data Cleaning Process

The dataset was inspected for common data quality issues including:

- Missing values
- Duplicate records
- Incorrect data types
- Cancelled transactions
- Non-positive quantities
- Non-positive unit prices
- Inconsistent text values

## Cleaning Actions

The following transformations were performed using Power Query:

1. Promoted the first row to column headers.
2. Reviewed and corrected data types.
3. Removed duplicate records.
4. Removed cancelled invoices.
5. Removed records with missing Customer IDs.
6. Removed records with non-positive quantities.
7. Removed records with non-positive unit prices.
8. Trimmed and cleaned text fields.
9. Performed another duplicate check after cleaning.
10. Created a Revenue column using Quantity × UnitPrice.
11. Set Revenue to Decimal Number data type.

## Final Dataset

The cleaned dataset contains:

- 392,692 rows
- 9 columns

The final columns are:

- InvoiceNo
- StockCode
- Description
- Quantity
- InvoiceDate
- UnitPrice
- CustomerID
- Country
- Revenue

No data errors were present in the final cleaned dataset.

## Purpose

The cleaned dataset will be used for exploratory data analysis,
business insights and the development of an interactive Power BI
dashboard.

## Next Step

The next stage of the project is Exploratory Data Analysis (EDA),
where the cleaned dataset will be analyzed to identify sales,
customer, product and geographic insights.
## Cleaned Dataset

The cleaned dataset contains 392,692 rows and 9 columns.

Due to the file size limitation on GitHub, the cleaned Excel dataset
is hosted on Google Drive.

[Download the Cleaned Dataset](https://docs.google.com/spreadsheets/d/11Ve6e2dgpOYlRJKvNHJAu6LVyuinpAJb/edit?usp=drivesdk&ouid=109913878589781834118&rtpof=true&sd=true)
## Task 2 — Exploratory Data Analysis

### Objective

The objective of this stage was to explore the cleaned Online Retail dataset, identify important trends and patterns, investigate potential anomalies, and generate useful business insights.

### Tools Used

- Microsoft Excel
- Power Query
- PivotTables
- PivotCharts
- Excel Slicers

### Dataset

The cleaned dataset contains:

- 392,692 rows
- 9 columns
- 4,338 customers
- 3,665 products
- 37 countries

### Key KPIs

| KPI | Value |
|---|---:|
| Total Revenue | 8,887,208.89 |
| Total Quantity Sold | 5,152,002 |
| Total Orders | 18,532 |
| Total Customers | 4,338 |
| Total Products | 3,665 |
| Total Countries | 37 |
| Average Order Value | 479.56 |

### EDA Performed

The analysis examined:

1. Monthly revenue trends
2. Top 10 products by revenue
3. Top 10 products by quantity sold
4. Top 10 countries by revenue
5. Top 10 customers by revenue
6. Potential transaction anomalies

### Key Insights

1. The United Kingdom generated approximately 82% of total recorded revenue, showing a strong concentration of revenue in the UK market.

2. Revenue generally increased toward the final quarter of 2011, with November 2011 recording the highest complete monthly revenue at 1,156,205.61.

3. Paper Craft, Little Birdie generated 168,469.60 in revenue, making it the highest-revenue product/description in the analysis.

4. Customer 14646 generated 280,206.02 in revenue, the highest recorded customer revenue.

5. A transaction involving Paper Craft, Little Birdie recorded 80,995 units, which represents a potential anomaly or bulk purchase requiring further investigation.

6. Customer 12346 generated 77,183.60 in revenue from a single order containing 74,215 units, another unusually large transaction that warrants investigation.

7. December 2011 contains data only through December 9, so its revenue should not be interpreted as a complete-month performance.

### Dashboard

An interactive Excel EDA dashboard was created containing:

- KPI summary
- Monthly revenue trend
- Top products by revenue
- Top products by quantity
- Top countries by revenue
- Top customers by revenue
- Interactive slicers
- Key insights
- Potential anomalies

### Project Progress

- [x] Task 1 — Data Cleaning & Preparation
- [x] Task 2 — Exploratory Data Analysis
- [ ] Task 3 — Interactive Dashboard
- [ ] Task 4 — Final Data Analytics Project

### Cleaned Dataset

The cleaned dataset is hosted on Google Sheets because of the large file size.

[View the Cleaned Dataset](https://docs.google.com/spreadsheets/d/11Ve6e2dgpOYlRJKvNHJAu6LVyuinpAJb/edit?usp=sharing&ouid=109913878589781834118&rtpof=true&sd=true))
