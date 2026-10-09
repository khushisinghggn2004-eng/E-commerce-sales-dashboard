# E-commerce-sales-dashboard 

##1.Project title
E-Commerce Sales Dashboard (Power BI)

##2.Short Description:
An interactive Power BI dashboard that analyzes e-commerce order data. It tracks four KPIs: total sales, number of orders, unique customers, and average order value (AOV). Each KPI shows month-over-month growth with green/red indicators. The report breaks sales down by product category, payment method, payment status, country and continent, using a donut chart, column chart, detail table, and slicers for filtering by month and other fields.

##3.Tech Stack:

- Power BI Desktop: report design, visuals, slicers, and the .pbit template
- Power Query (M): loading the CSV source and cleaning it (typing, promoting headers)
-DAX: measures such as Sales, Orders, AOV, Customers, previous-month comparisons (PREVIOUSMONTH), growth %, and conditional color logic. A calculated date table is built with CALENDARAUTO().
-Data modeling: a star schema with the ecommerce_data fact table linked to dimension tables for product, payment method, payment status, country, and a calendar
-CSV: the source data (ecommerce_data.csv)
