## Hi there 👋

<!--
**Mohmedafroz/mohmedafroz** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
--> # 📊 Week 1 — Excel-Based Sales Dashboard
### Data Analytics Internship | Domain: AI & DATA

---

## 🎯 Objective

Analyze a retail sales dataset and build a complete 
professional Excel dashboard showing:
- Total Sales Performance
- Monthly Revenue Trends  
- Top Products by Revenue
- Regional Sales Breakdown

---

## 🛠 Tools & Techniques Used

| Tool / Concept | Usage |
|----------------|-------|
| Microsoft Excel | Primary tool for data and dashboard |
| SUMIF | Revenue aggregation by month, product, region |
| IFERROR | Clean error handling in all formulas |
| INDEX + MATCH | Dynamic lookups for KPI cards |
| RANK | Product and region ranking |
| AVERAGE | Performance metrics |
| Line Chart | Monthly revenue trend visualization |
| Bar Chart | Product revenue comparison |
| Pie Chart | Quarterly revenue split |
| Horizontal Bar | Region-wise unit comparison |
| Conditional Formatting | Color scales and data bars |
| Auto Filter | Interactive data exploration |

---

## 📂 Sheets Overview

| Sheet | Purpose |
|-------|---------|
| 📊 Dashboard | Executive view — 4 KPI cards + 5 live charts |
| 📋 Sales Data | 38 raw transactions with auto revenue formula |
| 📅 Monthly | Month-wise revenue, MoM growth %, cumulative total |
| 🏆 Products | Product ranking by revenue and share % |
| 🌍 Regions | Region-wise performance and revenue breakdown |

---

## 📊 Dashboard Preview

![Dashboard](screenshots/01_Dashboard.png)

---

## 📸 All Sheets

### 📋 Sales Data
![Sales Data](screenshots/02_Sales_Data.png)

### 📅 Monthly Analysis  
![Monthly](screenshots/03_Monthly.png)

### 🏆 Product Performance
![Products](screenshots/04_Products.png)

### 🌍 Regional Breakdown
![Regions](screenshots/05_Regions.png)

---

## 🔑 Key Business Insights

| Insight | Value |
|---------|-------|
| 💰 Total Annual Revenue | ₹1,90,18,500 |
| 📦 Total Units Sold | 1,147 units |
| 🏆 Top Product | Laptop (56.4% revenue share) |
| 🌍 Best Region | East (₹74,38,500 — 39.1% share) |
| 📅 Best Month | December (₹31,45,000) |
| 📉 Weakest Month | April (₹7,55,000) |
| 📈 Biggest MoM Growth | September (+115% over August) |
| 🔋 Year-End Demand | December = 16.5% of full year revenue |

---

## 📈 Formula Reference

```excel
-- Revenue per order
= Units * Unit Price

-- Monthly revenue total
= SUMIF(Month_Column, "January", Revenue_Column)

-- Month-over-Month Growth %
= IFERROR((This_Month - Last_Month) / Last_Month, 0)

-- Cumulative Revenue
= SUM($Revenue$First : Revenue_This_Row)

-- Product Rank
= RANK(This_Revenue, All_Revenue_Range, 0)

-- Revenue Share %
= IFERROR(This_Revenue / SUM(All_Revenue), 0)

-- Top Product (KPI Card)
= INDEX(Product_Range, MATCH(MAX(Revenue_Range),
        Revenue_Range, 0))
```

---

## 📁 File Structure
