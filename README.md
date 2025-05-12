# Pizza Sales Analysis – Real-Time BI Project using MySQL & Power BI

This is a real-time data analytics project based on pizza sales, completed using **MySQL** for backend data querying and **Power BI** for frontend dashboard creation and storytelling. The project focuses on business KPIs, visual insights, and performance trends across categories, sizes, days, and months.

---

##  Project Objective

Analyze pizza sales data to extract actionable business insights — such as identifying best-selling products, busiest time periods, and overall category performance — through professional BI dashboards and SQL-based analysis.

---

##  Tools & Technologies

- **MySQL** – For writing queries and calculating KPIs
- **Power BI** – For creating dashboards and visual storytelling
- **DAX** – For calculated measures and sorting in Power BI
- **MS Word** – For documentation of SQL queries

---

Dashboards Overview- 

 Dashboard 1: Sales Performance & Time Trends
Key KPIs:

 Total Revenue

 Total Pizzas Sold

 Total Orders

 Average Order Value

 Average Pizzas per Order

Key Visuals:

 Donut Chart: Sales % by Pizza Category

 Donut Chart: Sales % by Pizza Size

 Bar Chart: Daily Trends (Orders by Day)

 Line/Bar Chart: Monthly Trends

 Card visuals: KPIs

 Dashboard 2: Best & Worst Sellers
Top Performers:

 Highest Revenue: Thai Chicken Pizza

 Most Quantity Sold: Classic Deluxe Pizza

 Most Orders: Classic Deluxe Pizza

Lowest Performers:

 Lowest Revenue: Brie Carre Pizza

 Least Quantity: Brie Carre Pizza

 Least Orders: Brie Carre Pizza

Key Visuals:

Bar charts for Top 5 & Bottom 5 by:

Revenue

Quantity Sold

Total Orders

KPIs & SQL Queries- 

1. Total Revenue:
sql
Copy
Edit
SELECT SUM(total_price) AS total_revenue FROM pizza_sales;
2. Average Order Value:
sql
Copy
Edit
SELECT SUM(total_price) / COUNT(DISTINCT order_id) AS avg_order_value FROM pizza_sales;
3. Total Pizzas Sold:
sql
Copy
Edit
SELECT SUM(quantity) AS pizza_sold FROM pizza_sales;
4. Daily Trend (by Weekday):
sql
Copy
Edit
SELECT DAYNAME(order_date) AS day_name, COUNT(DISTINCT order_id) AS total_orders
FROM pizza_sales
GROUP BY day_name
ORDER BY day_name;

Full list of 16+ queries is available in the included .docx file.




                       
