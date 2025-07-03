# Online Retail Sales Analysis (SQL Project)

This project explores online retail sales data using SQL, focusing on customer behavior, revenue trends, product performance, and segmentation.

##  Key Insights

- **Customer Segmentation:** One-time, repeat, and high-value buyers  
- **Revenue Analysis:** Top countries and customer spend  
- **Top Products:** Most purchased items and category-level sales  
- **Sales Trends:** Monthly patterns to identify seasonality  
- **Customer Value:** Highest lifetime spend per customer

##  Dataset & Tools

- **Source:** Online Retail dataset (UCI/Kaggle)  
- **Table:** `online_retail`  
- **Tools:** SQL (GROUP BY, CASE, JOIN, ORDER BY)

## Sample SQL Highlights

```sql
-- Segment customers
SELECT CustomerID, COUNT(DISTINCT InvoiceNo), 
CASE 
  WHEN COUNT(*) = 1 THEN 'OneTime' 
  WHEN COUNT(*) <= 6 THEN 'Repeat' 
  ELS
