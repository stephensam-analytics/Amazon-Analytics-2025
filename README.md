# 🛒 Amazon Sales Data Analysis (SQL)

## 📊 Project Overview
This project uses SQL to analyze Amazon sales data and answer key business questions about revenue, product categories, customers, payment methods, and order cancellations.

The aim was to turn raw order data into clear insights that can help a business make better decisions.

## 📂 Dataset
The dataset (`amazon_sales_data`) contains about 250 orders, with information on:

* Order ID and order date
* Products and product categories
* Price and quantity ordered
* Customer name and customer location
* Payment method
* Order status (Completed, Pending, Cancelled)

## 🧹 Data Preparation
Before analysis, the data was checked and prepared by:

* Checking the number of rows and distinct values
* Reviewing the order status values (Completed, Pending, Cancelled)
* Checking for missing values and duplicates
* Calculating revenue as `price * quantity`

## 🔍 Analysis Performed
The analysis was done with 18 SQL queries, grouped by topic.

**Sales performance**
* Total number of orders and total revenue
* Revenue by product category
* Percentage contribution of each category to total revenue
* Average order value per category
* Monthly sales trend and month-over-month revenue growth

**Products**
* Distinct product categories
* Top 5 most expensive products
* Ranking of products by total revenue (window function: `RANK()`)

**Customers**
* Top 5 customers by amount spent
* First and most recent order per customer
* Repeat customers (more than 3 orders)
* Revenue by customer location

**Orders and payments**
* Most popular payment method
* Count of cancelled orders (77 out of about 250)
* Cancellation rate by category
* Orders grouped into Low, Medium and High value tiers (`CASE WHEN`)

## 💡 Key Insights

* Total revenue generated was **[total_revenue]** across **[total_orders]** orders.
* **[Top category]** was the highest-earning category, contributing **[X]%** of total revenue.
* **77 orders (about 30%)** were cancelled, worth **[cancelled_total]** in lost sales.
* **[Top payment method]** was the most popular payment method.
* **[Top location]** generated the most revenue.
* Revenue was strongest in **[best month]** and weakest in **[weakest month]**.
* **[Customer name]** was the top customer, spending **[amount]**.

## 🎯 Business Recommendations

* Focus marketing and stock on **[top category]**, which drives the most revenue.
* Investigate why so many orders are cancelled, starting with **[category with highest cancellation rate]**.
* Promote the most popular payment method to make checkout smoother.
* Reward repeat customers with offers to increase loyalty.
* Use the monthly trend to plan inventory for stronger and weaker periods.

## 🛠️ Tools Used

* SQL (MySQL)
* MySQL Workbench
* Aggregate functions: `SUM`, `COUNT`, `AVG`, `MIN`, `MAX`
* `GROUP BY`, `HAVING`, `ORDER BY`
* `CASE WHEN`
* Window functions: `RANK()`, `LAG()`
* CTEs (`WITH`)

## 👨‍💻 About Me
**Samuel Kayode**
Data Analyst | Excel | SQL | Power BI
Turning raw data into meaningful insights and better decisions.
