 **Product Analytics Dashboard**

## 📌 Project Overview
The **Product Analytics Dashboard** is designed to provide actionable insights into product performance, sales trends, and discount effectiveness.  
By visualizing the data in **Power BI** and storing it efficiently using **SQL Server**, this project empowers management teams to make **data-driven decisions**.

The dashboard provides a comprehensive view of:
- Revenue performance across countries and time periods.
- Year-over-Year (YoY) growth in revenue and profit.
- The impact of discount strategies on overall revenue.
- A detailed table breakdown of revenue and profit at multiple levels.

This project was built to support **strategic decision-making** by tracking key performance metrics and identifying opportunities for growth.

---

## 📜 Problem Statement
The management team requested a **high-level dashboard** to track key product metrics and evaluate performance trends.

### **Business Requirements**
The dashboard must include:

1. **Revenue by Country**  
   Identify top-performing regions and their corresponding revenue.

2. **Revenue by Date and Year**  
   Compare revenue trends over different years and months.

3. **Profit and Unit Sales YoY Change**  
   High-level summary of growth in profit and units sold.

4. **Revenue Breakdown by Discount Band**  
   Analyze how discounts are impacting total revenue.

5. **Detailed Table View**  
   Breakdown of revenue and profit by country and year.


## 🗂 Dataset Information
The analysis uses three key datasets. These datasets were imported into **SQL Server** for cleaning, transformation, and integration.

| Dataset Name          | Description |
|-----------------------|-------------|
| **Product_data.csv**  | Contains product-level information such as product name, category, and price. |
| **discount_data.csv** | Includes discount details such as discount band and percentage discount. |
| **product_sales.csv** | Contains sales transactions including date, quantity sold, total revenue, and profit. |

### **Sample Fields**
- **Product_data.csv** → `Product_ID`, `Product_Name`, `Category`, `Unit_Price`  
- **discount_data.csv** → `Product_ID`, `Discount_Band`, `Discount_Percentage`  
- **product_sales.csv** → `Order_ID`, `Date`, `Product_ID`, `Quantity_Sold`, `Revenue`, `Profit`, `Country`

---

## 🛠 Tools & Technologies
| Tool / Technology  | Purpose |
|--------------------|---------|
| **SQL Server**     | Database creation, data storage, and transformations (ETL process). |
| **Power BI**       | Dashboard development and data visualization. |
| **Excel / CSV**    | Raw data storage and initial exploration. |

---

## ⚙️ Project Workflow

### **Step 1 – Load Data into SQL Server**
1. Create a new database named `ProductAnalytics`.
2.Import CSV files into their respective tables using **SQL Server Management Studio (SSMS)**.
3. Written a SQL query to load the desired data into power BI.

### **Step 2 – Connect Power BI to SQL Server**
- Connect Power BI to SQL Server using the database credentials.
- Used a query to load only desired data instead of entire dataset.
- Load the transformed tables into Power BI.

### **Step 4 – Build the Dashboard in Power BI**

| Visual Type    | Purpose |
|----------------|---------|
| **KPI Cards**  | Display key metrics like Total Revenue, Total Profit, Units Sold, YoY Growth % |
| **Bar Chart**  | Revenue by Country |
| **Line Chart** | Monthly Revenue Trend |
| **Donut Chart**| Revenue Breakdown by Discount Band |
| **Matrix Table** | Revenue and Profit by Country and Year |
| **Tooltips** | Provide detailed insights on hover |

### **Step 5 – Final Dashboard Layout**
The dashboard consists of **two pages**:
1. **Dashboard** – Main page with KPIs and visuals.  
2. **Tooltip Page** – Provides detailed drill-through insights.

---

## 📊 Key Insights

Here are some key takeaways derived from the dashboard:

### **Top Performing Countries**
- The **United States**, **Germany**, and **France** generate the highest revenue.

### **Revenue Trends**
- Significant increase observed in **2023**, indicating overall business growth.

### **Discount Impact**
- **High discount bands** contributed the most to revenue but decreased overall profit margins.

### **Year-over-Year Growth**
- Overall **34% increase in profit** compared to the previous year.
