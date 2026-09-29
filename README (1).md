# 🍕 Pizza Sales Performance Dashboard

> **A SQL + Power BI business intelligence project focused on turning pizza sales data into actionable sales, product, and customer-order insights.**

![Pizza Sales Performance Dashboard](assets/pizza_sales_dashboard.png)

## 📌 Project Overview

This project analyzes pizza sales performance to understand **how the business is performing across revenue, orders, products, categories, sizes, and ordering patterns**.

The analysis combines **Excel for initial data exploration**, **SQL for data cleaning and analytical queries**, and **Power BI for interactive data visualization and dashboard development**.

The final dashboard brings the most important KPIs and business questions into a single management-style view, making it easier to identify revenue drivers, popular products, demand patterns, and lower-performing products.

---

## 🎯 Business Objective

The goal of this project was to build a practical BI solution that answers questions such as:

- How much revenue is the business generating?
- How many orders and pizzas are being sold?
- What is the average order value?
- How many pizzas are purchased per order?
- Which days and months have the highest order volume?
- Which pizza categories contribute the most sales?
- Which pizza sizes generate the most revenue?
- Which individual pizzas are the strongest and weakest performers?
- Which products should receive further investigation for pricing, promotion, inventory, or product-positioning decisions?

---

## 📊 Key Performance Indicators

| KPI | Result |
|---|---:|
| **Total Revenue** | **$817,860.05** |
| **Total Orders** | **21,350** |
| **Total Pizzas Sold** | **49,574** |
| **Average Order Value** | **$38.31** |
| **Average Pizzas per Order** | **2.32** |

These figures are calculated from the `pizza_sales` dataset using `SUM(total_price)`, `COUNT(DISTINCT order_id)`, and `SUM(quantity)`.

---

## 🔎 Key Business Insights

### 1. Daily ordering pattern

**Friday** recorded the highest number of orders at **3,538**, while **Sunday** recorded the lowest at **2,624**.

This highlights a difference in order demand across the week and creates a useful basis for staffing, inventory planning, and promotional analysis.

### 2. Monthly demand variation

**July** had the highest order volume with **1,935 orders**, while **October** had the lowest with **1,646 orders**.

Understanding month-level variation can help support seasonal planning and campaign timing.

### 3. Sales contribution by pizza category

The four categories are relatively balanced:

| Category | Share of Sales |
|---|---:|
| **Classic** | **26.91%** |
| **Supreme** | **25.46%** |
| **Chicken** | **23.96%** |
| **Veggie** | **23.68%** |

Classic pizzas contributed the largest share of sales at **26.91%**, while the remaining categories were relatively close in contribution.

### 4. Pizza size is a major revenue driver

**Large pizzas generated 45.89% of sales**, followed by **Medium pizzas at 30.49%**.

This provides a clear view of customer demand by pizza size and can inform product mix and inventory planning.

### 5. Product performance differs by metric

The analysis evaluates product performance using **revenue, quantity sold, and order count** separately.

- **The Thai Chicken Pizza** generated the highest revenue: **$43,434.25**.
- **The Classic Deluxe Pizza** recorded the highest quantity sold: **2,453 pizzas**.
- **The Classic Deluxe Pizza** also recorded the highest number of orders: **2,329**.
- The analysis separately identifies the bottom-performing pizzas by revenue, quantity, and order count.

---

## 🛠️ Tools & Technologies

### Excel
Used for:
- Initial data exploration
- Understanding dataset structure and quality
- Supporting early-stage analysis

### SQL
Used for:
- Data cleaning
- KPI calculations
- Aggregation and grouping
- Trend analysis
- Category and size analysis
- Top/Bottom product analysis
- Distinct order analysis

### Power BI
Used for:
- Data modeling
- DAX measures
- Time-intelligence analysis
- KPI cards
- Interactive filters and slicers
- Dashboard design
- Business-oriented data storytelling

---

## 🧠 Analytical Approach

The project followed a practical BI workflow:

**Raw Sales Data → Excel Exploration → SQL Cleaning & Analysis → Power BI Data Model → DAX Measures → Interactive Dashboard → Business Insights**

The objective was to move from **transaction-level data to a decision-oriented business report**.

---

## 📈 Dashboard Components

The dashboard consolidates multiple analytical perspectives into a single page.

### KPI Layer
- Total Revenue
- Total Pizza Sold
- Total Orders
- Average Order Value

### Trend Analysis
- Sales and order trends over time
- Order-volume patterns across the week

### Category Analysis
- Sales contribution by pizza category
- Orders by pizza category

### Size Analysis
- Revenue contribution by pizza size

### Product Performance
- Top 5 pizzas by revenue
- Product-level sales, order count, and average-order-value comparison
- Identification of lower-performing products

---

## 🧮 SQL Analysis Highlights

The SQL work focused on answering business questions through aggregation and comparative analysis.

Example: total orders

```sql
SELECT COUNT(DISTINCT order_id) AS Total_Order
FROM pizza_sales;
```

Example: average pizzas per order

```sql
SELECT
    SUM(quantity) / COUNT(DISTINCT order_id) AS Avg_pizza_per_order
FROM pizza_sales;
```

The project also used:
- `SUM()`
- `COUNT(DISTINCT ...)`
- `GROUP BY`
- `ORDER BY`
- `LIMIT`
- `ROUND()`
- `DAYNAME()`
- `MONTHNAME()`
- Percentage-of-total calculations

---

## 💡 Business Value

The analysis can support decisions around:

- **Inventory planning** based on demand patterns
- **Promotional campaigns** around higher-order periods
- **Product positioning** using revenue and popularity metrics
- **Sales strategy** using category, size, and product performance
- **Further product investigation** for lower-performing items

---

## 🎓 Skills Demonstrated

### Business Intelligence
- KPI development
- Sales performance analysis
- Trend analysis
- Product performance analysis
- Business-question-driven reporting

### SQL
- Aggregations
- Grouping and sorting
- Distinct-count analysis
- Percentage-of-total calculations
- Top/Bottom analysis
- Date-based analysis

### Power BI
- Data modeling
- DAX measures
- Time intelligence
- Interactive slicers/filters
- KPI cards
- Dashboard design
- Data storytelling

### Data Analysis
- Excel-based exploration
- Data cleaning
- Translating business questions into analytical queries
- Turning analytical outputs into stakeholder-friendly visuals

---

## 🚀 Project Outcome

This project demonstrates an end-to-end BI workflow where **SQL is used to investigate and analyze transactional sales data, while Power BI is used to turn those findings into an interactive management dashboard**.

The focus is on connecting:

**KPIs → Trends → Product Performance → Business Questions → Insights**

This project is intended to demonstrate hands-on capability in **SQL + Power BI**, supported by Excel-based exploration.

---

## 👤 Target Role

**Junior BI Analyst**

Relevant skills demonstrated:

**SQL | Power BI | DAX | Data Analysis | Business Intelligence | Dashboard Development | KPI Reporting**

---

## 📌 Project Source

The dataset/project was developed from a **YouTube-based learning project** and analyzed using Excel, SQL, and Power BI.

> **Portfolio note:** This project is presented as a practical BI case study demonstrating hands-on SQL analysis, data modeling, DAX, and Power BI dashboard development.
