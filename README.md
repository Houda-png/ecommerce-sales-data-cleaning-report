# E-commerce Sales Data Cleaning & Reporting

## Project Overview

A U.S. e-commerce company provides a messy Excel file containing customer and order data.

The goal of this project is to clean, validate and transform the dataset, calculate useful business metrics, and generate a professional Excel report that can be used for analysis.

## Input File

`messy_sales_orders.xlsx`

The original dataset contains 65 rows and 18 columns, including:

- Customer information
- Contact details
- Location data
- Product information
- Quantity and pricing
- Discounts
- Order dates
- Payment methods
- Order statuses

The dataset intentionally contains data-quality issues such as missing values, inconsistent text formats, invalid values and duplicate order IDs.

## Data Cleaning & Validation

The Python pipeline performs the following operations:

- Detects missing values
- Detects duplicate order IDs
- Removes unnecessary whitespace
- Standardizes U.S. state names and abbreviations
- Standardizes payment methods
- Standardizes order statuses
- Normalizes email addresses
- Standardizes phone numbers
- Validates email formats
- Validates phone numbers
- Validates customer ages
- Validates quantities
- Validates unit prices
- Validates discount percentages
- Separates valid and invalid records
- Records validation issues for invalid rows

## Business Metrics

For valid orders, the project calculates:

- Gross amount
- Discount amount
- Net amount
- Total revenue
- Average order value
- Number of completed orders
- Number of pending orders
- Number of cancelled orders
- Revenue by product
- Revenue by state

## Final Results

After validation:

- 50 valid records
- 15 invalid records
- Total revenue: $4,495.60
- Average order value: $89.91

## Output File

`clean_sales_report.xlsx`

The final Excel workbook contains three worksheets:

### Clean Orders
Validated and cleaned order data with calculated financial columns.

### Invalid Records
Rejected records together with the reason each record failed validation.

### Summary
Key business metrics, revenue by product, and revenue by state.

## Excel Formatting

The final workbook is formatted with `openpyxl` and includes:

- Styled headers
- Borders
- Automatic column sizing
- Frozen header rows
- Filters
- Currency formatting

## Technologies Used

- Python
- pandas
- openpyxl
- Jupyter Notebook

## Repository Files

- `sales_data_cleaning.ipynb` — complete data cleaning and reporting pipeline
- `messy_sales_orders.xlsx` — sample messy input dataset
- `clean_sales_report.xlsx` — final professional Excel report
