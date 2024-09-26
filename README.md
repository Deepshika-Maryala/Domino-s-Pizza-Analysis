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
Select sum(total_price) as Total_Revenue from pizza_sales;
```
![Screenshot 2024-09-26 161651](https://github.com/user-attachments/assets/6cc18174-59c4-404f-b104-f89251db3a81)

```sql
Select count(distinct(order_id)) as Total_Order from pizza_sales;
```
![Screenshot 2024-09-26 161907](https://github.com/user-attachments/assets/a85010eb-29a5-4610-adbd-e5d1ff6aeaf1)

```sql
Select sum(quantity) as Total_Pizza_sold from pizza_sales;
```
![Screenshot 2024-09-26 161931](https://github.com/user-attachments/assets/488a864e-6739-4fb0-aa28-38ab11ce80d7)

```sql
Select (sum(total_price)/count(distinct(order_id))) as Average_Order_Value from pizza_sales;
```
![Screenshot 2024-09-26 161955](https://github.com/user-attachments/assets/9d319cbd-5e97-431c-af06-a0b7b853e475)

```sql
Select (sum(quantity)/count(distinct(order_id))) as Average_pizzas_per_order from pizza_sales;
```
![Screenshot 2024-09-26 162020](https://github.com/user-attachments/assets/143dd980-acb8-4719-968a-54c9af80dca2)

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
## Report Snapshots (Power BI Desktop):

![Screenshot 2024-09-26 163300](https://github.com/user-attachments/assets/aeae4d67-a4be-40a5-b4d4-2d0d23a600f2)



![Screenshot 2024-09-26 163448](https://github.com/user-attachments/assets/8e18632f-42fd-4c41-999d-218131302086)





