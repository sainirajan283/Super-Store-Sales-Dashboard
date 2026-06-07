# 🛒 SuperStore Sales Dashboard — Power BI

A comprehensive **sales analytics dashboard** built in Power BI, featuring interactive visuals and a **15-Day Sales Forecast** to support data-driven business decisions.

---

## 📊 Project Overview

This project analyzes retail sales data from a fictional SuperStore to uncover trends in revenue, profit, customer segments, and regional performance. The report is designed to help business stakeholders quickly identify top-performing categories, monitor KPIs, and forecast near-future sales.

---

## 🖥️ Dashboard Pages

### Page 1 — Sales Overview Dashboard
An interactive summary of overall business performance, including:
- Total Sales, Total Profit, Total Orders, and Average Delivery Days (KPI cards)
- Sales by **Category** and **Sub-Category**
- Sales by **Customer Segment** (Consumer, Corporate, Home Office)
- Sales by **Payment Mode** (Online, Cards, COD)
- Sales by **Region** (Central, East, South, West)
- Monthly **Sales** and **Profit** trends (Year-over-Year comparison)
- Sales distribution by **Ship Mode**

### Page 2 — 15-Day Sales Forecast
A time-series forecasting page built using Power BI's built-in analytics:
- Historical daily sales trend line
- **15-day forward forecast** with confidence interval bands
- State-level sales breakdown for granular regional analysis

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Power BI Desktop** | Dashboard development & visualization |
| **Power Query** | Data cleaning and transformation |
| **DAX** | Custom measures and calculated columns |
| **Excel / CSV** | Source data |

---

## 📐 Key DAX Measures Used

```dax
-- Average Delivery Days
Avg Delivery Days = AVERAGEX(Orders, Orders[Ship Date] - Orders[Order Date])

-- Sales YoY
Sales YoY = CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Calendar'[Date]))
```

---

## 📁 Project Structure

```
Super-store-sales-dashboard/
│
├── Super-store-sales-dashboard.pbix   # Main Power BI report file
├── README.md                          # Project documentation
└── dataset/
    └── SuperStore_Sales_Dataset.csv   # Source data (if included)
```

---

## 🔍 Key Insights

- **Consumer segment** contributes the highest share of total sales (~48%)
- **Cash on Delivery (COD)** is the most preferred payment mode
- **West region** leads in sales volume across all categories
- **Office Supplies** is the top-selling category by order volume
- The 15-day forecast suggests a **moderate upward trend** in sales heading into the next period

---

## 🚀 How to Use

1. Download and install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
2. Clone or download this repository
3. Open `Super-store-sales-dashboard.pbix` in Power BI Desktop
4. Interact with slicers (Region, Year, Category) to filter the visuals
5. Navigate to **Page 2** to explore the 15-Day Sales Forecast

---

## 🎯 Skills Demonstrated

- Data cleaning and shaping with **Power Query**
- Writing custom **DAX measures** (time intelligence, aggregations)
- Designing an intuitive, business-ready **BI dashboard**
- Applying **forecasting analytics** in Power BI
- Storytelling with data across multiple report pages

---
