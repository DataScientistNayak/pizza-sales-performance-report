# 🍕 Pizza Sales Performance Dashboard

An interactive **Pizza Sales Performance Dashboard** built using **PostgreSQL** and **Power BI** to analyze sales trends, customer ordering patterns, product performance, and business insights.

This project transforms raw pizza sales data into meaningful visual insights using SQL for data extraction and Power BI for dynamic dashboard creation.

---

## 📌 Project Overview

The main objective of this project is to analyze pizza sales data and provide actionable insights through an interactive dashboard.

The dashboard helps in:

- Tracking overall sales performance
- Understanding customer ordering behavior
- Identifying top-performing and low-performing pizzas
- Analyzing sales distribution by category and size
- Monitoring monthly and daily sales trends

---

## 🎯 Problem Statement

The business wants to analyze pizza sales performance to improve revenue generation and optimize product strategy.

### KPI Requirements

| KPI | Description |
|------|------------|
| Total Revenue | Sum of the total price of all pizza orders |
| Total Orders | Total number of orders placed |
| Average Order Value | Total Revenue ÷ Total Orders |
| Total Pizzas Sold | Sum of all pizzas sold |
| Average Pizzas Per Order | Total Pizzas Sold ÷ Total Orders |
<img width="407" height="238" alt="Screenshot 2026-06-23 221630" src="https://github.com/user-attachments/assets/ca7f58da-8c75-42ab-b43f-9882feee90c4" />

---

## 📊 Dashboard Requirements

### Charts & Analysis

- **Monthly Revenue Trend** → Analyze revenue performance across different months
- **Daily Trend for Total Orders** → Understand customer ordering behavior throughout the week
- **Percentage of Sales by Pizza Category** → Category-wise contribution to total sales
- **Percentage of Sales by Pizza Size** → Size-wise contribution to total sales
- **Total Pizzas Sold by Size and Category** → Comparative sales volume analysis
- **Revenue by Pizza Name** → Individual pizza revenue contribution
<img width="401" height="230" alt="Screenshot 2026-06-24 080302" src="https://github.com/user-attachments/assets/f539607a-b48f-4ba2-9965-3af788f35c23" />

---

## 🔍 Top & Bottom Analysis

The dashboard identifies:

### Best Performers
- Top Pizza by Revenue
- Top Pizza by Orders
- Top Pizza by Quantity Sold

### Poor Performers
- Worst Pizza by Revenue
- Worst Pizza by Orders
- Worst Pizza by Quantity Sold

---

## 🛠 Tech Stack

- **Database:** PostgreSQL
- **Visualization Tool:** Power BI
- **Query Language:** SQL
- **Data Source:** Pizza Sales Dataset (CSV)
<img width="401" height="230" alt="Screenshot 2026-06-24 080320" src="https://github.com/user-attachments/assets/050e7474-a513-4d59-b7b6-a21a0fc7c597" />

---

## ⚙ Workflow

### 1. Data Collection
Imported pizza sales CSV dataset into PostgreSQL.

### 2. Data Cleaning
- Checked missing values
- Corrected column mismatches
- Standardized data types

### 3. Data Analysis using SQL
Performed KPI calculations:

```sql
-- Total Revenue
SELECT SUM(total_price) FROM pizza_sales;

-- Total Orders
SELECT COUNT(DISTINCT order_id) FROM pizza_sales;

-- Average Order Value
SELECT SUM(total_price)/COUNT(DISTINCT order_id) FROM pizza_sales;

-- Total Pizzas Sold
SELECT SUM(quantity) FROM pizza_sales;

-- Average Pizzas Per Order
SELECT SUM(quantity)/COUNT(DISTINCT order_id) FROM pizza_sales;
```

### 4. Power BI Dashboard Creation
Connected PostgreSQL database with Power BI and created interactive visualizations.
<img width="598" height="370" alt="Screenshot 2026-06-24 235204" src="https://github.com/user-attachments/assets/ab0e79f5-8c27-440e-9e79-60042e96ffde" />

---

## 📈 Key Insights

- Highest revenue generated in **July**
- Maximum orders observed on **Thursday**
- **Large size pizzas** contributed the highest sales percentage
- **Classic category pizzas** generated the highest revenue share
- Top-performing pizza identified through revenue, orders, and quantity analysis

---

## ✨ Features

✔ Interactive Filters (Month, Category, Size)  
✔ Dynamic KPI Cards  
✔ Revenue Trend Analysis  
✔ Order Pattern Analysis  
✔ Category-wise Sales Analysis  
✔ Size-wise Sales Analysis  
✔ Top & Bottom Product Analysis  
✔ Treemap for Revenue by Pizza Name  

---

## 📷 Dashboard Preview

### Main Dashboard
(Add your dashboard screenshot here)

```md
![Dashboard](images/dashboard.png)
```

### KPI Requirements
```md
![KPI Requirements](images/kpi_requirements.png)
```

### Chart Requirements
```md
![Chart Requirements](images/chart_requirements.png)
```

### Top & Bottom Analysis
```md
![Top Bottom Analysis](images/top_bottom_analysis.png)
```

---

## 🚀 How to Run This Project

### PostgreSQL Setup

1. Create database:
```sql
CREATE DATABASE pizza_sales;
```

2. Import CSV file into PostgreSQL.

3. Run SQL queries for analysis.

---

### Power BI Setup

1. Open `PIZZA SALES DASHBOARD.pbix`
2. Connect it to your PostgreSQL database
3. Refresh the dataset
4. Explore the dashboard

---

## 💡 Business Impact

This dashboard helps businesses:

- Identify best-selling pizzas
- Optimize inventory management
- Improve pricing strategy
- Enhance customer satisfaction
- Increase revenue through data-driven decisions

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Smruti Ranjan Nayak**  
B.Tech CSE | Data Science Enthusiast | Power BI Developer
