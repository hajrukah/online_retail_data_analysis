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
