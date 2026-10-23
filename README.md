# Sales_Performance_Net_Profit_tracker
Sales Tracker Analysis project that helps organizations monitor sales, calculate net profit over time, and identify profit trends using PowerBI for data cleaning and visualization.
# Departmental Business - Net Profit Analysis

## 📌 About The Project
This project focuses on calculating the net profit of a departmental business using sales data. The analysis was carried out by comparing the **Total Cost Price** and the **Total Selling Price** for all transactions.

The main goal was to help the business understand its overall profitability over time and to identify which department was more **productive and efficient** in generating profit.

## 🎯 Objectives
- Calculate Total Sales, Total Cost, and Net Profit
- Track profit trends over time
- Compare departmental performance based on profit contribution
- Highlight the most efficient and least efficient departments

## 📊 Dataset
- **File:** data/Semantic_Sales.csv (60k+ transactions)
- **Columns:** OrderDate, ProductKey, Quantity, Unit Price, Sales, Cost
- **New Calculated Column:** Net Profit = Sales - Cost

## 🛠️ Tools Used
- Microsoft Excel (Data Cleaning, Formulas, Pivot Tables)
- Power BI (Data Modeling, DAX, Dashboard & Visualizations)

## 🔑 Key Calculations
- `Total Sales = Quantity * Selling Price`
- `Total Cost = Quantity * Cost Price`
- `Net Profit = Total Sales - Total Cost`
- `Profit Margin % = (Net Profit / Total Sales) * 100`

## 📈 Key Insights
- Identified total net profit generated over the period
- Determined the most productive and profitable department
- Visualized profit trends to support business decision-making

## 💡 Recommendation
Insights from this analysis can help management make better decisions on resource allocation, pricing strategy, and departmental improvement.

## 👤 Author
**Okusanya Oladayo Oluwaseun**  
Data Analyst | [LinkedIn](https://linkedin.com/in/oladayo-okusanya)

## 🧹 Data Cleaning & Preparation (ETL in Power BI)

All data cleaning and transformation was performed using **Power Query Editor in Power BI**.

**ETL Process:**

1.  **Data Profiling:** Performed initial data profiling to understand data distribution, column quality, and data types.
2.  **Source Connection:** Connected to **SQL Server** database as the data source.
3.  **Promoted Headers:** Promoted the first row to headers to ensure correct column naming.
4.  **Removed Unwanted Rows:** Removed the first top row and the bottom five rows which contained irrelevant totals/footers.
5.  **Query Management:** Renamed queries for better organization and readability.
6.  **Handled Faulty Columns:** Identified and removed faulty/irrelevant columns that were not needed for analysis.
7.  **Created Date Column:** Used **Column From Examples** to merge Month and Year columns to create a proper date dimension for time-series analysis.

After this cleaning process, the dataset was ready for modeling and profit calculation.
