# Car Sales Dashboard | Power BI

### An end-to-end Power BI analytics dashboard for the automotive retail industry.

<a href="https://app.powerbi.com/view?r=eyJrIjoiNWYwM2MyZTUtNGU3Mi00MzhlLWIwZGMtNzM3MGFkYmI5MjQ3IiwidCI6ImIxMGVjNzYyLTA1NjEtNDVmZS1iN2NmLWFjMWI4MzZkZTI3NyIsImMiOjF9">
  <img src="https://github.com/AmitKPandeyLabs/PowerBI_3_Car_Sales_Dashboard/raw/main/Project3_Car_Sales_Dashboard.png" alt="Car Sales Dashboard" width="800">
</a>

### [Click Here (Ctrl+Click opens new tab) to View the Interactive Dashboard](https://app.powerbi.com/view?r=eyJrIjoiNWYwM2MyZTUtNGU3Mi00MzhlLWIwZGMtNzM3MGFkYmI5MjQ3IiwidCI6ImIxMGVjNzYyLTA1NjEtNDVmZS1iN2NmLWFjMWI4MzZkZTI3NyIsImMiOjF9)

<br>

## 📈 Project Overview

This Power BI project provides a comprehensive analysis of car sales data. The solution ingests data from multiple disparate sources, transforms it into a clean star schema model, and presents it in a dynamic, multi-page interactive dashboard. The report empowers sales directors, regional managers, and marketing teams to analyze performance by company, body style, region, and time, enabling data-driven decisions to optimize sales and pricing strategies.

## 🎯 Objectives

-	Analyze Year-to-Date (YTD) and Month-to-Date (MTD) performance for key metrics: Total Sales, Cars Sold, and Average Price.
-	Measure and compare Year-over-Year (YoY) growth to identify trends and assess business health.
-	Provide a geographical breakdown of sales performance by dealer and region using an interactive map.
-	Segment sales by key vehicle attributes: Body Style, Color, Transmission, and Engine type.
-	Identify top-performing car companies and their contribution to total sales.
-	Enable deep-dive analysis through interactive slicers for granular insights.

## 🔍 Key Dashboard Features

**Key KPIs:**
- **YTD Total Sales:** $371.2M (with 23.59% YoY growth)
- **YTD Avg Price:** $28.0K (with -0.79% YoY change)
- **YTD Cars Sold:** 13.3K (with 24.57% YoY growth)
- **MTD KPIs:** Month-to-Date analysis for Total Sales ($54.28M), Avg Price ($28.26K), and Cars Sold (1.92K).

**Time Series Analysis:**
-	`YTD Sales Weekly Trend` (Area Chart): Visualizes performance over the year, highlighting a significant peak around week 40 (14.9M).

**Categorical Breakdown (Donut Charts):**
-	`YTD Total Sales by Body Style`: Provides a clear view of market demand (e.g., SUV, Hatchback, Sedan).
-	`YTD Total Sales by Color`: Shows customer color preferences (e.g., Pale White, Black, Red).

**Geospatial Analysis (Map):**
-	`YTD Cars Sold by Dealer, Region`: An interactive map of the United States with bubble sizes representing sales volume at key dealer locations (Pasco, Aurora, Janesville, etc.).

**Company Performance (Matrix):**
-	A detailed table of `Company Wise Sales Trend` showing YTD Avg Price, Cars Sold, and Total Sales for each brand.
-	Features an in-visual `%GT YTD Total Sales` bar chart to quickly identify top-contributing companies.

**Interactive Slicers:**
-	A dedicated filter pane to drill down into the data by `Body Style`, `Dealer_Name`, `Transmission`, and `Engine`.

## 💡 Notable Insights

-	The business is experiencing strong **Year-over-Year growth**, with YTD Cars Sold up 24.57% and Total Sales up 23.59%.
-	The **Average Price has remained stable** (down only -0.79% YoY), indicating that growth is driven by volume, not just price inflation.
-	Sales are seasonal, with a significant **peak around week 40** (14.9M), which can inform inventory and marketing strategies.
-	**SUVs** are the most popular body style, driving a substantial portion of total sales.
-	The matrix reveals different company strategies: some brands (like **Volvo**) have a high average price ($27.9K) and lower volume, while others (like **Toyota**) achieve high total sales ($17.5M) through greater volume (593 cars sold).

## 🛠️ Tools & Skills Demonstrated

-	**Power BI Desktop**: Data Import (multiple CSVs), Data Modeling, Visualization.
-	**Power Query (ETL)**: Connected to 10+ disparate flat files, performed extensive data cleaning and transformation (handling nulls, changing data types), and merged queries to create a robust **star schema data model**.
-	**Data Modeling**: Built relationships between the central `Sales` (Fact) table and `Cars`, `Dealers`, `Company`, and `Color` (Dimension) tables to enable efficient and accurate analysis.
-	**DAX (Data Analysis Expressions)**: Authored complex time-intelligence measures from scratch, including:
    - `YTD Total Sales` & `MTD Total Sales` (using `TOTALYTD`, `TOTALMTD`)
    - `YTD Cars Sold` & `MTD Cars Sold` (using `CALCULATE`, `COUNTROWS`, `DATESYTD`, `DATESMTD`)
    - `Previous Year YTD Sales` & `YoY Sales %` (using `SAMEPERIODLASTYEAR` and `BLANK` to handle nulls)
-	**Dashboard Design (UI/UX)**: Created a multi-page report with a clean, professional UI, including a main "Overview" page for high-level KPIs and a "Details" page for granular analysis.
-	**Power BI Service**: Published the final report to the web to enable live, interactive stakeholder access.

## 🚀 Usage

1. **[Launch (Ctrl+Click opens new tab) the interactive dashboard](https://app.powerbi.com/view?r=eyJrIjoiNWYwM2MyZTUtNGU3Mi00MzhlLWIwZGMtNzM3MGFkYmI5MjQ3IiwidCI6ImIxMGVjNzYyLTA1NjEtNDVmZS1iN2NmLWFjMWI4MzZkZTI3NyIsImMiOjF9)**.
2. Use the slicers on the left pane to filter the entire report by `Body Style`, `Dealer_Name`, `Transmission`, or `Engine`.
3. Click on any element (e.g., "SUV" in the donut chart or "Toyota" in the table) to cross-filter all other visuals on the page.
4. Hover over data points to see detailed tooltips and values.
