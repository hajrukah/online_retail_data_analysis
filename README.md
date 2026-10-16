# Online Retail Sales Analysis
### From Data Cleaning to Exploratory Analysis and Interactive Power BI Dashboard

## Project Overview
This project follows an end-to-end data analytics workflow using an Online Retail transaction dataset. It covers data cleaning and preparation, exploratory data analysis (EDA), KPI development, and an interactive Power BI dashboard.

## Problem Statement
Raw retail transaction data can contain duplicates, cancelled invoices, missing customer identifiers, inconsistent text, and unsuitable data types. Without structured analysis and reporting, it is harder to identify leading products, valuable customers, important markets, and revenue trends. This project prepares the data and presents findings through an interactive dashboard.

## Dataset Information
The dataset was sourced from Kaggle's Online Retail dataset.

The cleaned dataset contains these nine fields:
`InvoiceNo`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `UnitPrice`, `CustomerID`, `Country`, and `Revenue`.

- **Reported rows:** 392,692
- **Columns:** 9
- **Tools:** Microsoft Excel, Power Query, Power BI, DAX
- **Revenue calculation:** `Quantity Ã UnitPrice`
**[Open the cleaned dataset on Google Sheets https://docs.google.com/spreadsheets/d/11Ve6e2dgpOYlRJKvNHJAu6LVyuinpAJb/edit?usp=drivesdk&ouid=109913878589781834118&rtpof=true&sd=true
## Task 1 â Data Cleaning and Preparation
The dataset was prepared using Microsoft Excel and Power Query. The recorded workflow included:
1. Promoted the first row to headers.
2. Reviewed and corrected data types.
3. Removed duplicate records.
4. Removed cancelled invoices.
5. Removed records with missing `CustomerID`.
6. Removed non-positive `Quantity` values.
7. Removed non-positive `UnitPrice` values.
8. Trimmed and cleaned text fields.
9. Performed an additional duplicate check after text cleaning.
10. Created `Revenue` using `Quantity Ã UnitPrice`.
11. Set `Revenue` to a decimal data type.

The final Power Query output was reported as 392,692 rows and 9 columns, with no errors in the final check.
## Task 2 â Exploratory Data Analysis
Excel PivotTables and PivotCharts were used to examine monthly revenue trends, top products by revenue and quantity, revenue by country, top customers by revenue, and unusually large transactions.

### Key metrics
| Metric | Previously calculated value |
|---|---:|
| Total Revenue | 8,887,208.89 |
| Total Quantity Sold | 5,152,002 |
| Distinct Orders | 18,532 |
| Distinct Customers | 4,338 |
| Distinct Product Codes | 3,665 |
| Countries | 37 |
| Average Order Value | 479.56 |

**Validation note:** Recheck these figures against the final Power BI report before publication, particularly if the source table or filters have changed.
## Task 3 â Interactive Power BI Dashboard
The Power BI report includes six KPI cards:
- Total Revenue
- Total Quantity
- Total Orders
- Total Customers
- Total Products
- Average Order Value

### Visualizations
- Monthly Revenue Trend
- Top 10 Countries by Revenue
- Top 10 Customers by Revenue
- Top 10 Products by Revenue
- Top 10 Products by Quantity Sold

### Interactive slicers
- Country
- Invoice Date
- Product Description

The slicers allow users to explore performance by market, time period, and product.
## Key Findings
These findings were recorded during the earlier EDA and should be checked against the final dashboard before submission.

1. **Revenue concentration:** UK revenue was previously calculated at approximately 7,285,024.64, around 82% of total recorded revenue.
2. **Monthly performance:** November 2011 revenue was previously calculated at approximately 1,156,205.61. December 2011 is incomplete because the dataset ends on December 9.
3. **Product performance:** `Paper Craft, Little Birdie` was previously reported at approximately 168,469.60 in revenue.
4. **Customer contribution:** Customer `14646` was previously reported at approximately 280,206.02 in revenue.
5. **Potential anomaly:** A transaction involving `Paper Craft, Little Birdie` was reported with 80,995 units. This may be a legitimate bulk purchase and should be investigated rather than automatically labelled an error.
6. **Period limitation:** December 2011 contains data only through December 9 and should not be compared directly with full months.

## Business Recommendations
- Investigate the drivers of the UK's revenue contribution and assess opportunities in other markets.
- Review the products and customer activity behind November's revenue peak.
- Use product findings to inform inventory and merchandising reviews alongside margin and stock availability data.
- Examine high-value customers' purchasing patterns for retention opportunities.
- Investigate unusually large transactions to distinguish bulk purchases from data or process issues.
- Compare monthly performance using complete periods or clearly label partial months.

## Limitations
- Revenue is not profit because costs and margins are not included.
- Large quantities are potential anomalies, not confirmed errors.
- The analysis identifies patterns but does not establish their causes.
- December 2011 is incomplete.
- Validate all KPI values against the final Power BI model before publication.
