# E-commerce-sales-dashboard 

##1.Project title
E-Commerce Sales Dashboard (Power BI)

##2.Short Description:
An interactive Power BI dashboard that analyzes e-commerce order data. It tracks four KPIs: total sales, number of orders, unique customers, and average order value (AOV). Each KPI shows month-over-month growth with green/red indicators. The report breaks sales down by product category, payment method, payment status, country and continent, using a donut chart, column chart, detail table, and slicers for filtering by month and other fields.

##3.Tech Stack:

- Power BI Desktop: report design, visuals, slicers, and the .pbit template
- Power Query (M): loading the CSV source and cleaning it (typing, promoting headers)
-DAX: measures such as Sales, Orders, AOV, Customers, previous-month comparisons (PREVIOUSMONTH), growth %, and conditional color logic. A calculated date table is built with CALENDARAUTO().
- Data modeling: a star schema with the ecommerce_data fact table linked to dimension tables for product, payment method, payment status, country, and a calendar
- CSV: the source data (ecommerce_data.csv)

 ##4.Features:
 1. Business Problem:
An e-commerce business collects thousands of order records, but raw CSV data doesn’t show how the business is performing. Leadership can’t easily see whether sales, orders, customers, and order value are growing or shrinking from month to month. They also can’t tell which products, payment channels, or regions drive revenue, or where payments are failing or stuck.

 2.Goal:
- Turn raw order data into a single-page, interactive dashboard that:
- Monitors key sales KPIs and their month-over-month change at a glance
- Shows revenue and order distribution across products, payment methods, payment status, and geography
- Lets stakeholders filter by time period and other dimensions without any technical work, so they can make faster data-driven decisions
 3.Walkthrough of Key Visuals
- Header and title banner: “E-Commerce Dashboard” with a themed background gives the report a clean, branded look.
- KPI cards (Sales, Orders, Customers, AOV): Each card shows the current value with a comparison against the previous month. The growth % is colored green for an increase and red for a decrease, driven by DAX color measures. A dynamic “VS [previous month]” label updates with the selected month. Small icons sit beside each card for quick recognition.
- Month slicer and button slicer: These let users filter the whole page by time period or category, so every KPI and chart recalculates instantly.
- Donut chart: Shows the proportional split of a categorical dimension, such as payment method, payment status, or category. It’s useful for spotting dominant segments.
- Clustered column chart: Compares sales or orders across categories or periods, making top and bottom performers easy to see.
- Detail table: A drill-down view of the underlying order-level data, so users can verify the numbers behind the visuals.
