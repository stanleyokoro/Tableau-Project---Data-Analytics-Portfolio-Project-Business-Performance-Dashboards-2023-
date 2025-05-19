# 📊 Business Performance Dashboards (2023)

**Author**: Stanley Chinor Okoro  
**Platform**: [Tableau Public](https://public.tableau.com/app/profile/stanley.okoro6105/viz/SalesCustomerDashboardsDynamic_17476654261050/SalesDashboard)  
**Tools Used**: Tableau, Calculated Fields, Logical Expressions  
**Project Type**: Data Analytics Portfolio  
**Focus Areas**: Year-over-Year KPI Analysis, Sales & Customer Trends, Strategic Insights

---

## 🎯 Project Overview

This project consists of two interactive Tableau dashboards—**Sales Dashboard** and **Customer Dashboard**—designed to uncover business insights from 2023. The dashboards provide comparative performance analysis against the previous year using custom-calculated KPIs, trendlines, and behavioral analytics.

---

## 📌 Key Features

- **Dynamic Year Filtering**  
  Enables year-over-year (YoY) comparisons between Current Year (CY) and Previous Year (PY).

- **Custom KPIs & Metrics**  
  - % Difference in Customers, Orders, Sales, Profit, Quantity
  - Sales per Customer and % YoY Change
  - KPI Flags for above/below average performance
  - Min/Max monthly metric highlighting

- **Interactive Dashboards**  
  - Monthly and weekly granularity
  - Product sub-category breakdown
  - Customer order behavior distribution
  - High-value customer profiling

---

## 📈 Dashboard Insights

### 🔹 Sales Dashboard
- **Total Sales**: $733K (+20.4% YoY)
- **Total Profit**: $93K (+12.5% YoY)
- **Quantity Sold**: 12K units (+26.8% YoY)
- **Trends**: Strong December finish; January was the weakest month.
- **Product Analysis**:
  - Top Sellers: Phones, Chairs, Binders
  - Highest Margin: Copiers
  - Loss Leaders: Accessories, Machines

### 🔹 Customer Dashboard
- **Total Customers**: 693 (+8.6% YoY)
- **Total Orders**: 1,687 (+28.3% YoY)
- **Sales/Customer**: $1,058 (+10.8% YoY)
- **Behavior Distribution**:
  - Majority place only 1–2 orders
  - Opportunity for loyalty and reactivation strategies
- **Top Customers by Profit**:
  - Raymond Buch, Hunter Lopez, Tom Ashbrook

---

## 🔍 Strategic Business Use Cases

- **Executive Summary KPIs**
- **Seasonal Pattern Recognition**
- **Customer Segmentation & Loyalty Design**
- **Profitability & Product Mix Optimization**
- **Sales vs. Profit Misalignment Detection**
- **Growth Levers for Marketing & Inventory Planning**

---

## 🛠️ Technical Highlights

### 📐 Key Calculated Fields

```tableau
// Year Definitions
Current Year = [Select Year]
Previous Year = [Select Year] - 1

// KPI Metrics
% Diff Customers = (COUNTD([CY Customers]) - COUNTD([PY Customers])) / COUNTD([PY Customers])
CY Sales per Customer = SUM([CY Sales]) / COUNTD([CY Customers])
PY Sales per Customer = SUM([PY Sales]) / COUNTD([PY Customers])
% Diff Sales per Customer = ([CY Sales per Customer] - [PY Sales per Customer]) / [PY Sales per Customer]

// KPI Flags
KPI CY Less PY = IF SUM([CY Sales]) < SUM([PY Sales]) THEN '⬤' ELSE '' END
KPI Sales Avg = IF SUM([CY Sales]) > WINDOW_AVG(SUM([CY Sales])) THEN 'Above' ELSE 'Below' END
```

### 📊 Visual Cues

- Above/Below Average Indicators
- Dynamic Year Filtering
- Monthly Min/Max Highlighters for Customers, Orders, Profit, Sales

---

## 📎 Access the Dashboards

🔗 [Sales & Customer Dashboards on Tableau Public](https://public.tableau.com/app/profile/stanley.okoro6105/viz/SalesCustomerDashboardsDynamic_17476654261050/SalesDashboard)

---

## 🧠 Portfolio Value

This project highlights my ability to:
- Build data products that blend strategic business thinking with analytical precision
- Design and implement custom KPIs
- Translate performance data into actionable insights
- Build dashboards for executive decision-making

---

## 📬 Contact

**Stanley Chinor Okoro**  
📧 Email: stanley.chinor@gmail.com  
🔗 LinkedIn: [timelesshov](https://www.linkedin.com/in/timelesshov)  
💻 GitHub: [timelesshov](https://github.com/stanleyokoro)
