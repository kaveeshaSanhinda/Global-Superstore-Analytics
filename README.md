# 🌍 Global Superstore Analytics — Power BI Dashboard

## 📌 Project Overview
An interactive 5-page Power BI dashboard built to analyze global sales, 
profit, customer segments, and shipping performance across 147 countries.

---

## 🎯 Objective
To transform raw transactional data into actionable business insights 
using data modeling, DAX calculations, and interactive visualizations.

---

## 🛠️ Tools & Technologies
- **Power BI Desktop** — Dashboard development
- **Power Query (M Language)** — Data cleaning & transformation
- **DAX** — KPI measures and time intelligence
- **Star Schema Modeling** — Fact & dimension table structure

---

## 📊 Dashboard Pages
| Page | Description |
|------|-------------|
| 1. Executive Summary | High-level KPIs — Sales, Profit, Orders |
| 2. Sales Analysis | Sales trends by region, category & segment |
| 3. Product Performance | Top/bottom products by profit margin |
| 4. Customer Insights | Customer segmentation and behaviour |
| 5. Shipping Analysis | Delivery performance by ship mode |

---

## 🧮 Key DAX Measures
```dax
Total Sales = SUM(FactOrders[Sales])

Total Profit = SUM(FactOrders[Profit])

Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)

YoY Sales Growth % = 
DIVIDE([Total Sales] - [Sales PY], [Sales PY], 0)

Sales PY = 
CALCULATE([Total Sales], SAMEPERIODLASTYEAR(DimDate[Date]))
```

---

## 🔍 Key Findings
- **Technology** is the highest revenue category but **Office Supplies** 
  has the best profit margin
- **APAC and EU** regions show the strongest YoY growth
- **Same Day shipping** has the lowest usage but highest satisfaction rate
- The **Consumer segment** accounts for over 50% of total orders

---

## 👩‍💻 Author
**Kaveesha Sanhinda** | BA Undergraduate
[LinkedIn](www.linkedin.com/in/kaveesha-sanhinda-662910373)
