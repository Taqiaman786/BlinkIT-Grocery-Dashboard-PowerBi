# BlinkIT-Grocery-Dashboard-PowerBi

🛒 Blinkit Grocery Sales Analysis – Power BI Dashboard


📌 Project Overview
This project presents a Power BI dashboard built using the Blinkit Grocery Dataset sourced from Kaggle.

The dashboard provides insights into:

•	Total Sales Performance

•	Product Category Performance

•	Outlet Establishment Trends

•	Outlet Size & Location Analysis

•	Customer Rating & Item Distribution The goal of this project is to analyze sales trends and business performance metrics to support data-driven decision-making.

________________________________________
📂 Dataset Information

•	Source: Kaggle

•	File Used: BlinkIT Grocery Data.xlsx

•	Domain: Retail / Grocery / FMCG

•	Total Records: 8,523 items

•	Key Fields:

o	Item Identifier

o	Item Type

o	Item Fat Content

o	Outlet Identifier

o	Outlet Establishment Year

o	Outlet Size

o	Outlet Location Type

o	Outlet Type

o	Item Visibility

o	Item MRP

o	Sales

o	Rating


🧹 Data Cleaning & Transformation (Power Query Steps)

All cleaning steps were performed in Power BI Power Query Editor and documented below:

1️⃣ Handling Missing Values

•	Checked null values in:

o	Outlet Size → Replaced missing values with "Unknown"

o	Ratings → Verified consistency

•	Ensured no null values in key numerical columns (Sales, MRP)

2️⃣ Standardizing Categorical Values

•	Standardized Item Fat Content

o	Combined values like:

	"LF", "Low Fat" → Low Fat

	"reg" → Regular

3️⃣ Data Type Corrections

•	Sales → Decimal Number

•	Item MRP → Decimal Number

•	Outlet Establishment Year → Whole Number

•	Rating → Decimal Number

4️⃣ Derived Measures (DAX Measures Created)

Total Sales = SUM('BlinkIT Grocery Data'[Sales])

Average Sales = AVERAGE('BlinkIT Grocery Data'[Sales])

No of Items = COUNT('BlinkIT Grocery Data'[Item Identifier])

Average Rating = AVERAGE('BlinkIT Grocery Data'[Rating])

________________________________________
📊 Dashboard Overview

The dashboard consists of KPI Cards, Charts, and Filters, ensuring no visual is omitted.
________________________________________
🔢 KPI CARDS (Top Section)

1️⃣ Total Sales

•	Value: $1M

•	Shows total revenue generated from all items.

2️⃣ Average Sales

•	Value: $141

•	Shows average revenue per item.

3️⃣ Number of Items

•	Value: 8,523

•	Total number of unique products.

4️⃣ Average Rating

•	Value: 3.9

•	Overall average product rating.

________________________________________
📈 VISUALS EXPLAINED
________________________________________
1️⃣ Outlet Establishment (Area Chart)

Type: Area Chart

Axis: Outlet Establishment Year

Values: Total Sales

Insight:

•	Sales trend over establishment years.

•	Peak sales observed around 2018 (~$205K).

•	Helps analyze performance by outlet age.

________________________________________
2️⃣ Fat Content (Donut Chart)

Type: Donut Chart

Legend: Low Fat vs Regular

Values: Total Sales

Insight:

•	Regular items contribute higher sales (~$776K).

•	Low Fat contributes (~$425K).

•	Indicates customer preference trend.

________________________________________
3️⃣ Fat by Outlet (Stacked Bar Chart)

Type: Clustered Bar Chart

Axis: Outlet Tier (Tier 1, 2, 3)

Legend: Fat Content

Values: Total Sales

Insight:

•	Tier 3 outlets generate highest revenue.

•	Regular fat items dominate across all tiers.

________________________________________
4️⃣ Item Type (Horizontal Bar Chart)

Type: Bar Chart

Axis: Item Type

Values: Total Sales

Top Performing Categories:

•	Fruits & Vegetables (~$0.18M)

•	Snack Foods (~$0.18M)

•	Household (~$0.14M)

Insight:

•	Essential & consumable items drive maximum revenue.
________________________________________
5️⃣ Outlet Size (Donut Chart)

Type: Donut Chart

Legend: Small / Medium / High

Values: Total Sales

Insight:

•	Medium outlets contribute highest (~$508K).

•	Small outlets contribute (~$445K).

•	High size outlets contribute (~$249K).

________________________________________
6️⃣ Outlet Location (Bar Chart)

Type: Horizontal Bar Chart

Axis: Tier 1, Tier 2, Tier 3

Values: Total Sales

Insight:

•	Tier 3 locations generate highest sales (~472K).

•	Tier 2 (~393K)

•	Tier 1 (~336K)

________________________________________
7️⃣ Outlet Type (Matrix Table)

Type: Matrix Table

Rows: Outlet Type

Columns:

•	Total Sales

•	No of Items

•	Average Sales

•	Average Rating

•	Item Visibility

Insight:

•	Supermarket Type1 has highest total sales (~$788K).

•	Grocery Store has highest number of items (1,083).

•	Ratings are consistent (~4).

________________________________________
🎛 Filter Panel (Slicers)

The left panel contains interactive slicers:

•	Outlet Location Type

•	Outlet Size

•	Item Type

•	Clear All Slicers Button

These enable dynamic filtering across all visuals.

________________________________________

🎯 Business Insights Derived

•	Tier 3 outlets are highest revenue generators.

•	Medium-sized outlets outperform others.

•	Regular fat products sell more than Low Fat.

•	Fruits, Snacks, and Household items are key revenue drivers.

•	Older establishments (2018 onwards) show higher sales performance.

________________________________________

🛠 Tools Used

•	Power BI Desktop

•	Power Query

•	DAX

•	Microsoft Excel

•	Kaggle Dataset
________________________________________

📌 How to Use This Dashboard

1.	Use slicers to filter by outlet size, type, or item category.
2.	Analyze KPIs for performance overview.
3.	Drill into item type for product-level insights.
4.	Compare outlet tiers and sizes for expansion strategy.

🚀 Conclusion
This Power BI dashboard provides a complete retail performance overview for Blinkit grocery data.

<img width="1273" height="720" alt="Screenshot 2026-02-12 201811" src="https://github.com/user-attachments/assets/3226d654-4695-4203-8692-6385180b34d1" />

