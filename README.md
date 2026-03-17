
## Ecommerce Sales Analysis using SQL

## Project Overview

This project is a complete end-to-end SQL analysis of an ecommerce sales dataset.The goal of the project is to convert raw sales data into meaningful business insights that helps understand overall performance, product contribution and regional trends.

Instead of focusing only on SQL syntax, this project emphasizes **business-driven analysis**
and follows a clean, industry-style project structure.

## Project Objective
- Analyze overall sales and profit performance
- Identify top-performing products
- Understand category-wise and region-wise contribution
- Practice real-world SQL workflow from raw data to insights
- Build a structured and reproducible analytics project 

## Dataset Description
The dataset contains ecommerce transaction-level data with the following fields:

- Order Date  
- Product Name  
- Category  
- Region  
- Quantity  
- Sales  
- Profit    

        The raw dataset is stored as a CSV file and imported into SQL Server for analysis.

## Tools & Technologies
- **SQL Server Management Studio 22 (SSMS)**
- **SQL** (SELECT, GROUP BY, ORDER BY, Aggregations)
- **CSV Flat File Import**
- **Excel** Dashboard for visualizing key KPIs such as Total Sales, Total Profit,
  Category-wise Sales, Region-wise Sales, and Top Products

## Project Structure
```
Ecommerce_SQL_Project/
│
├── Data/
│   └── ecommerce_sales.csv
│
├── Queries/
│   ├── 01_total_sales.sql
│   ├── 02_total_profit.sql
│   ├── 03_category_sales_profit.sql
│   ├── 04_region_sales_profit.sql
│   ├── 05_top_10_products_sales_profit.sql
│   └── 06_time_based_analysis.sql
│
├── Results/
│   ├── 01_total_sales.csv
│   ├── 02_total_profit.csv
│   ├── 03_category_sales.csv
│   ├── 04_category_profit.csv
│   ├── 05_region_sales.csv
│   ├── 06_region_profit.csv
│   ├── 07_top_10_products.csv
│   └── 08_top_products_sales.csv
│
└── README.md  
```

## Folder Explanation
## 🔹 Data
Contains the raw ecommerce sales CSV file.
This file acts as the source data and is not modified during analysis.

## 🔹 Queries
Includes all SQL queries written for analysis.
Each query is saved separately and numbered to maintain execution order
and make the analysis easy to understand and reproduce.

## 🔹 Results
Stores the output generated from SQL queries.
Each result is exported as a CSV file, making it easy to use for Excel or Power BI dashboards.


Key Analysis Performed
- Total Sales calculation
- Total Profit calculation
- Category-wise Sales and Profit analysis
- Region-wise Sales and Profit analysis
- Top 10 Products based on total sales

## Sample SQL Query
```sql
SELECT TOP 10
    Product_Name,
    SUM(Sales) AS Total_Sales
FROM ecommerce_sales
GROUP BY Product_Name
ORDER BY Total_Sales DESC;
```

## Business Insights

- Identified products contributing the highest revenue
- Analyzed which categories and regions perform best
- Provided a clear overview of sales and profit distribution
- Created structured outputs ready for visualization


## What Makes This Project Strong
- End-to-end workflow from raw CSV to final insights
- Focus on business KPIs, not just SQL syntax
- Clean and professional folder structure
- Real-world problem-solving during data import and debugging
- Results exported in dashboard-ready format

## Excel Dashboard
An interactive Excel dashboard was created to visualize:
- Total Sales and Total Profit KPIs
- Category-wise Sales performance
- Region-wise Sales distribution
- Top 10 Products by Total Sales

## Author 
Sadhna

Aspiring Data Analyst

Skills: SQL | Excel | Data Analysis | Business Insights
