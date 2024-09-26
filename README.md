# Domino’s Pizza Sales Trends and Insights
### Project Overview:
This project aims to create a Power BI dashboard for Domino’s Pizza, offering real-time insights into key metrics such as total sales, total orders, total pizza sold, average order values and average pizza  per order. The dashboard will consolidate data from various sources, providing actionable insights.
### Purpose and Performance Targets:
- Design and develop an interactive sales overview dashboard and products overview dashboard.
- Monitor total sales performance across various time periods (daily, monthly).
- Analyze the performance of different pizza flavors, side items, and promotions to adjust offerings based on popularity.
### Data Source:
Sales data: The primary dataset used for analysis is the “pizza_sales.xlsx” file, containing detail information of Pizza sales.
### Tools
- Excel spreadsheets – Data cleaning
- SQL – Data Analysis
- Power BI Desktop [version 2.126.927.0] – Creating report
### Exploratory Data Analysis:
EDA involved exploring the sales data to answer the key questions such as:
- What are the overall sales trends (daily, monthly)?
- What are the top-selling pizza types and menu items?
- How do sales differ between weekdays and weekends?
### Data Analysis:
Analyzing Total revenue , total orders, total pizza sold, average order value and Average pizzas per order using SQL.
```sql
Select sum(pizza_sales) as Total Revenue from pizza_sales;
```
```sql
Select count(distinct(order_id)) as Total Order from pizza_sales;
```
```sql
Select sum(quantity) as Total Pizza sold from pizza_sales;
```
```sql
Select (sum(pizza_sales)/count(distinct(order_id))) as Average Order Value from pizza_sales;
```
```sql
Select (sum(quantity)/count(distinct(order_id))) as Average pizzas per order from pizza_sales;
```
### Insights And Findings:
- Sales have been highest mainly on friday and saturday in evenings.
- Large size pizza has contributes to maximum sales and total orders. 
### Analyzes Metrics:
- Total Revenue
- Total Pizza Sold
- Total orders
- Average Order Value
- Average pizzas per order
### Visuals and Dashboards:
#### Sales Dashboard:
- KPI: Total revenue, total orders, total pizza sold, average pizza per order and average order value.
- Daily Sales Trend: Analyzing the sales of the current month on daily basis.
- Monthly Sales Trend: Analyzing the sales of the current month on monthly basis.
- Total Pizza Sold by Pizza category: Analyzing category-wise total pizza sold.
- Total Revenue by Pizza Size: Analyzing the sales based on pizza size.
- Total Revenue by Pizza category: Analyzing the sales Based on pizza category.
#### Product Dashboard:
- KPI: Total revenue, total orders, total pizza sold, average pizza per order and average order value.
- Top 5 best sellers by total revenue: Analyzing the sales of the top 5 best selling pizzas.
- Top 5 best sellers by total quantity: Analyzing the total quantity of the top 5 best selling pizzas.
- Bottom 5 best sellers by total revenue: Analyzing the sales of bottom 5 best selling pizzas.
- Bottom 5 best sellers by total quantity: Analyzing the total quantity of the bottom 5 best selling pizzas.
### User Interactive features:
- Filters: Allows the user to filter by pizza category.
- Slicers: Provide options for different time periods (days, months).
### Project Phases And Milestones:
- Data Collection and Preparation: May 2024
- Dashboard Design and Development: July 2024





