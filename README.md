# Power BI E-Commerce Sales Dashboard

## Overview
Interactive sales dashboard built in Power BI analyzing 541,909 real 
transactions from a UK-based e-commerce store (1 year of data).

## Key Business Insights
- Total Revenue: 9.75M | Total Orders: 26K | Total Customers: 4K
- Revenue peaks in August-September — summer demand drives more 
  sales than the holiday season for this store
- United Kingdom accounts for 8.2M (84% of total revenue)
- Netherlands has the highest Average Order Value at 2.8K — 
  despite lower total orders, customers spend significantly more per order
- Top product: DOTCOM POSTAGE at 0.21M revenue

## Dashboard Visuals
- KPI Cards — Total Revenue, Total Orders, Total Customers
- Revenue by Month — line chart showing seasonal trends
- Top Products by Revenue — bar chart (sorted descending)
- Total Revenue by Country — bar chart
- Average Order Value by Country — bar chart (DAX measure)

## DAX Measures Used
- Total Revenue = SUM(data[Revenue])
- Total Orders = DISTINCTCOUNT(data[InvoiceNo])
- Total Customers = DISTINCTCOUNT(data[CustomerID])
- Avg Order Value = DIVIDE([Total Revenue], [Total Orders])

## Tools Used
Power BI Desktop, DAX, Data Cleaning, Data Modeling

## Dataset
E-Commerce Data — Kaggle (UCI Online Retail)
