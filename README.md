# Mobile_Sales_Dashbord

# 📱 Mobile Sales Analysis - Power BI Dashboard

## 🧠 Project Summary
This Power BI report analyzes **Mobile Sales Performance** across multiple time frames and dimensions.  
The goal is to provide business leaders with a clear view of sales patterns and help drive data-informed decisions.  
The analysis covers **City-wise breakdown**, **MTD (Month-To-Date)**, **QTD (Quarter-To-Date)**, **YTD (Year-To-Date)**, and comparisons with **Same Period Last Year (SPLY)**.

---

## 📂 Dataset Details
- **Source:** [Add source or say "Self-created Excel file"]
- **File Type:** Excel / CSV
- **Columns Example:**
  - `Order Date`
  - `City`
  - `Product`
  - `Quantity`
  - `Unit Price`
  - `Revenue`
  - `Customer Segment`

---

## 📌 Key Objectives
- Track mobile sales across various cities
- Compare current performance vs last year
- Enable time-based filtering (MTD, QTD, YTD)
- Provide actionable insights via dashboards

---

## 📊 Dashboard Breakdown
1. **📍 City-Wise Sales Overview**
   - Total Revenue by City
   - Top 5 Performing Cities
   - City Filter/Slicer

2. **⏱️ Time-Based Performance**
   - MTD / QTD / YTD Sales KPIs
   - Sales Growth vs Last Year
   - Monthly & Quarterly Trends

3. **📈 Comparative Analysis**
   - Same Period Last Year (SPLY) vs Current
   - Year-over-Year (YoY) growth
   - Product Category Sales Trends

---

## 🧮 DAX Measures Used
```DAX
MTD Sales = TOTALMTD(SUM(Sales[Revenue]), Sales[Order Date])
YTD Sales = TOTALYTD(SUM(Sales[Revenue]), Sales[Order Date])
QTD Sales = TOTALQTD(SUM(Sales[Revenue]), Sales[Order Date])
SPLY Sales = CALCULATE(SUM(Sales[Revenue]), SAMEPERIODLASTYEAR(Sales[Order Date]))
YoY Growth = DIVIDE([YTD Sales] - [SPLY Sales], [SPLY Sales])


📣 Connect With Me
Linkdin : www.linkedin.com/in/noman-mahmood-295220264
Email: nomanmahmood730@gmial.com

🏷️ Tags
#PowerBI #SalesAnalysis #MobileData #TimeIntelligence #BusinessIntelligence
