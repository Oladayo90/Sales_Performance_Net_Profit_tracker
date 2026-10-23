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

## 🔍 Exploratory Data Analysis (DAX Measures)

After cleaning, I created key performance measures using **DAX in Power BI** to analyze business performance.

#DAX Measures Created:


Here is the polished markdown for this new section - with the correct DAX formulas employers will understand:
🔍 Exploratory Data Analysis (DAX Measures)

After cleaning, I created key performance measures using **DAX in Power BI** to analyze business performance.

**DAX Measures Created:**

1.  **Total Revenue**
    ```DAX
    Total Revenue = SUM(Sales[Sales])
2.  *Total Cost*
    Total Cost = SUM(Sales[Cost])
3.  *Net Profit*
    Net Profit = [Total Revenue] - [Total Cost]
4.  *Profit Margin %*
    Profit Margin % = DIVIDE([Net Profit], [Total Revenue]) * 100
5.  *Average Monthly Profit*
    Avg Monthly Profit = AVERAGEX(VALUES('Date'[MonthYear]), [Net Profit])
These measures were used to build visuals to track overall profitability and identify the most productive department.

**Pro Tip:** I used `DIVIDE()` for Profit Margin instead of `/` - it prevents errors when sales is zero. That's best practice in Power BI and interviewers love it.

---

Do you want me to now combine EVERYTHING into **one final complete README.md** file?

1. About the project
2. Data Cleaning (ETL)
3. This DAX Analysis section
4. Your name & LinkedIn

So you can just paste once and your GitHub is done?
