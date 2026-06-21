1. Title & Badges

Project name: Data Mart - Weekly Sales Analysis

2. Project Overview

This project analyzes weekly retail and e-commerce sales data using MySQL. It covers data cleaning, transformation, and business insights across regions, platforms, customer segments, and time periods.

3. Dataset Description

The dataset weekly_sales contains transactional data with the following columns:

week_date- Date of the sales week
region- Geographic region (ASIA, AFRICA, USA, etc.)
platform- Sales platform (Retail / Shopify)
segment- Customer segment code
customer_type- New / Existing / Guest
transactions - Number of transactions
sales - Total sales amount.

4. Data Cleaning
   
A cleaned table clean_weekly_sales was created with additional derived columns:

week_number - Week number extracted from week_date
month_number- Month number extracted from week_date
calender_year - Year extracted from week_date
age_band- Derived from segment (Young Adults / Middle Age / Retirees)
demographic- Derived from segment (Couples / Families / Unknown)
avg_transac- Average transaction value (sales / transactions)

5. Business Questions Solved

1. Missing Week Numbers

Identified which week numbers (1–52) are absent from the dataset using:


Recursive CTE
UNION-based number table
NOT EXISTS
LEFT JOIN

2. Total Transactions per Year

Aggregated transaction counts grouped by calendar year.

3. Total Sales by Region and Month

Breakdown of sales performance across regions on a monthly basis.

4. Platform Transaction Count

Compared transaction volumes between Retail and Shopify.

5. Retail vs Shopify Sales Percentage per Month
6. 
Calculated percentage share of sales for each platform per month using:

CASE WHEN (pivot style)
JOIN with subquery
Window Functions

6. SQL Concepts Used

✅ Data Cleaning & Transformation
✅ Window Functions (SUM OVER PARTITION BY)
✅ CASE WHEN (Pivot)
✅ LEFT JOIN / NOT EXISTS
✅ Aggregate Functions
✅ Round
✅ Where clause


7. Author:
Arindam Das
arindam0098@gmail.com
LinkedIn- https://www.linkedin.com/in/arindam-das-057158190/





