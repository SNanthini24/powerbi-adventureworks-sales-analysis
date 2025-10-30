# 📊 Power BI Project: Adventure Works Sales Analysis

## 🧠 Project Overview  
This Power BI dashboard analyzes the **Adventure Works** dataset — a fictional company that manufactures and sells cycling-related products globally.  
The project aims to uncover insights into **sales performance, product profitability, customer demographics, and regional trends**.

---

## 🗂️ Dataset & Source Information  
**Source:** Microsoft Adventure Works Sample Data  
**File Type:** Excel based dataset (converted for Power BI)  

**Key tables used:**  
- `Sales` – Transactional data including product, date, and revenue details  
- `Customers` – Demographic details of customers  
- `Products` – Product categories, subcategories, and cost details  
- `Territory` – Region and country mapping  
- `Calendar` – Date intelligence for time-based analysis  

---

## 🧰 Tools & Technologies Used  
- **Power BI Desktop** (for dashboard creation and analysis)  
- **Power Query** (for data cleaning and transformation)  
- **DAX (Data Analysis Expressions)** (for calculated columns and measures)  
- **Microsoft Excel** (for data preparation)  

---

## 📈 Dashboard Features & Sections  

### 🔹 Sales Overview  
- KPIs: Total Revenue, Total Profit, and Order Quantity  
- Year-over-Year (YoY) Sales Growth  
- Top performing regions and product categories  

### 🔹 Product Performance  
- Product category contribution to total sales  
- Profit margin by subcategory  
- Interactive filters for category and region  

### 🔹 Customer Insights  
- Customer segmentation by geography, gender, and age  
- Average revenue per customer  
- Repeat customer trends  

### 🔹 Regional Sales  
- Map visualization of sales by region   

---

## 🧮 Sample DAX Measures  
```DAX
Total Sales = SUM(Sales[SalesAmount])

Total Profit = SUM(Sales[Profit])

YoY Sales Growth % = 
VAR CurrentYear = CALCULATE([Total Sales], YEAR('Calendar'[Date]) = MAX('Calendar'[Year]))
VAR PreviousYear = CALCULATE([Total Sales], YEAR('Calendar'[Date]) = MAX('Calendar'[Year]) - 1)
RETURN DIVIDE(CurrentYear - PreviousYear, PreviousYear)
```

💡 Key Insights

📈 Sales increased by ~12% YoY, with highest growth in North America.

💰 Mountain Bikes contribute the most to revenue but have moderate profit margins.

👩‍💼 Male customers aged 30–45 are the top buyers.

🌍 The United States leads in total sales among all regions.

📁 Project Files

AdventureWorks_Analysis.pbix — Power BI project file

AdventureWorks_Data.csv — Cleaned dataset

README.md — Documentation (this file)

📂 Download and explore the Power BI dashboard from the link below:

https://1drv.ms/u/c/13dddcd7d54447e8/EdXUCObf-Z5EjWzW2mVRcEQBjW2GxOVc6y-Gwr8KaLz3wg?e=1zHAn6

🖼️ Dashboard Preview

📊 Sales Overview
├── Executive_Dashboard.jpg
👥 Customer Insights
├── Customer_Dashboard.jpg
🛍️ Product Performance
├── Product_Dashboard.jpg
🌍 Regional Sales
└── Map.jpg

🚀 How to Use

1. Download the .pbix file using the link above.

2. Open it in Power BI Desktop (latest version recommended).

3. Explore the visuals, slicers, and filters to uncover insights.

🧑‍💻 Author

Nanthini S
Aspiring Data Analyst | SQL | Power BI | Excel | Python

📧 nanthinisakthinathan@gmail.com

