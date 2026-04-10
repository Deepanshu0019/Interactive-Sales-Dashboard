👟 Adidas US Sales Performance Dashboard

US_Sales.pbix (Power Bi)

<img width="480" height="480" alt="Screenshot 2026-04-09 152544" src="https://github.com/user-attachments/assets/d27e50d1-eaab-48b6-bf83-71116248a256" />

📌 Project Overview

This project analyzes Adidas US sales data to uncover regional performance, top-selling products, channel contributions and growth trends over time. The goal is to provide a clear, data-driven view of sales performance that helps business stakeholders make quick decisions.

🎯 Key KPIs
MetricValue💰 Total Sales Revenue$127.4M📈 YoY Growth Rate+29.2%🛒 Average Order Value$187.50🎯 Sales vs Target112.5%

📊 Dashboard Highlights

Sales by Region — West Coast leads, followed by Northeast & Midwest
Sales by Product Category — Footwear dominates over Apparel & Accessories
Sales Trend Over Time — Monthly revenue growth from Jan–Aug 2025
Top 5 Products by Revenue — Ultra Boost, NMD, Stan Smith & more
Sales by Channel — Wholesale (31%), E-Commerce (40%), Direct-to-Consumer (30%)
Regional Market Share — Interactive donut chart for all US regions
Sales Performance vs Target — Gauge chart showing 112% achievement


🔍 Key Insights

📍 West Coast generates the highest regional revenue
👟 Footwear is the top-performing product category
🌐 E-Commerce channel contributes the largest share at ~40%
📈 Consistent month-over-month growth throughout 2025
🎯 Overall sales exceeded target by 12.5%
🥇 Ultra Boost 23 Black is the #1 product by revenue


🛠️ Tools & Technologies
ToolUsagePower BIDashboard design, DAX measures, slicers & filtersMicrosoft ExcelData source, cleaning & preprocessingDAXCustom KPI calculations, YoY growth, % measures

📐 DAX Measures Used
dax-- Total Sales Revenue
Total Sales = SUM(adidas_sales[Total_Sales])

-- Year-over-Year Growth
YoY Growth % =
  DIVIDE(
    [Total Sales] - CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Date'[Date])),
    CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Date'[Date]))
  ) * 100

-- Sales vs Target %
Sales vs Target % =
  DIVIDE([Total Sales], [Sales Target]) * 100

-- Average Order Value
Avg Order Value = DIVIDE([Total Sales], COUNTROWS(adidas_sales))

📁 Project Structure
Adidas-US-Sales-Dashboard/
│
├── 📊 Adidas_Sales_Dashboard.pbix   # Power BI file
├── 📋 adidas_us_sales.xlsx          # Raw dataset
├── 🖼️ dashboard_preview.png         # Dashboard screenshot
└── 📄 README.md

🚀 How to Use

Clone this repository

bash   git clone https://github.com/Deepanshu0019/Adidas-US-Sales-Dashboard.git

Open adidas_us_sales.xlsx to explore the raw data
Open Adidas_Sales_Dashboard.pbix in Power BI Desktop
Use the slicers to filter by Date Range, Region, Product Category and Sales Channel
Hover over charts to see detailed tooltips


🖼️ Dashboard Preview

Interactive filters available for:

📅 Start & End Date
🗺️ Region (All / West Coast / Northeast / Midwest / Southeast / Southwest)
👕 Product Category (Footwear / Apparel / Accessories)
🏪 Sales Channel (Wholesale / E-Commerce / Direct-to-Consumer)



👨‍💻 Author
Deepanshu Mehta
📧 deepanshu9469@gmail.com
🔗 LinkedIn
🐙 GitHub

⭐ If you found this project helpful, please give it a star!
