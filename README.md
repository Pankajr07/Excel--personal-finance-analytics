# Personal Finance Analytics – Excel Project

An Excel-based personal finance dashboard analyzing **11 months of transaction data**.  
Includes data cleaning, category mapping, monthly summaries, and dynamic PivotTable-driven visualizations.

---

## 📂 File Overview

**Main Excel File:**  
➡️ [Personal Finance Project.xlsx](Personal%20Finance%20Project.xlsx)

This workbook contains:

- raw + cleaned transaction data  
- category mappings  
- monthly summaries  
- PivotTables  
- an interactive dashboard

---

## 📄 Key Sheets

### **1. Personal spending**
Core transaction table with:

- Date  
- Month-year (e.g. `2025-01`)  
- Unique ID  
- Tran Type (e.g. EFTPOS)  
- Payee (raw bank description)  
- Merchant (cleaned, standardised name)  
- Category (e.g. Groceries, Dining, Transport, etc.)  
- Memo  
- Amount (negative = spending, positive = income)  
- Type (`in` / `out`)

This sheet contains **220 transactions** across **11 months**, grouped into **16 categories** and **76 merchants**.

---

### **2. MerchantMapping**
Cleaning table used to standardise messy merchant names into consistent labels.

---

### **3. Category by Month-Year**
Aggregated table summarising **total spending per category per month**.  
Used as a source for charts and the dashboard.

---

### **4. Pivot Tables**
PivotTables used to:

- calculate total income & total spending  
- break down spending by category  
- rank merchants by spend  
- summarise monthly trends

---

### **5. Income Sparklines**
Mini line charts to compare income/spending trends over time.

---

### **6. Dashboard**
A clean dashboard displaying:

- KPI cards (Income, Spending, Net Balance)  
- Monthly spending trend chart  
- Category breakdown chart  
- Summary visuals

---

## 📊 Metrics & Insights

From this analysis:

- **Total Income:** 7,126.90  
- **Total Spending:** 6,133.86  
- **Net Balance:** 993.04  

The dashboard answers questions such as:

- Which months had the highest spending?  
- Which categories take up most of my money?  
- Which merchants do I spend the most at?  
- How does spending change month-to-month?

---

## 📌 Data Notes (Important)

**Cash income is intentionally excluded from this analysis.**  
Reliable historical records for cash earnings were not available, and adding estimated values would reduce the accuracy and integrity of the results.

To maintain clean, verifiable, and fully reproducible insights, this dashboard focuses exclusively on **bank-recorded electronic transactions** with consistent timestamps, descriptions, and amounts.

A future enhancement may introduce a manual cash-logging sheet if reliable entries become available.

---

## 🧹 Data Cleaning & Preparation

Key steps performed:

- Imported bank transaction exports  
- Created a `Month-year` field for grouping  
- Standardised merchant names using mapping table  
- Categorised each transaction  
- Corrected transaction signs (income vs spending)  
- Built structured tables connected to PivotTables

---

## 🛠 Excel Techniques Used

- Structured Tables  
- PivotTables  
- `SUMIFS` and other formula-based metrics  
- Custom month-year grouping  
- Dashboard design using:  
  - column, line, and donut charts  
  - summary KPI cells  
  - PivotTable references  

---

## 🚀 Future Improvements

- Export cleaned data into SQL Server  
- Rebuild analysis in SQL (CTEs, aggregates, window functions)  
- Build a Power BI dashboard  
- Add advanced metrics such as:  
  - savings rate %  
  - category trends over time  
  - month-over-month % changes  

---

## 🎯 Purpose

This project is part of my analytics portfolio as an **aspiring Data / Reporting Analyst**.

It demonstrates my ability to:

- work with real financial data  
- clean and structure messy exports  
- build meaningful summaries  
- visualize insights clearly  
- explain spending patterns and behaviour  

---

