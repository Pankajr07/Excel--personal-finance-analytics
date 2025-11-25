# Excel--personal-finance-analytics
An Excel-based personal finance dashboard analyzing 11 months of transaction data. Includes data cleaning, category mapping, monthly summaries, and dynamic PivotTable-driven visualizations.
# Personal Finance Analytics – Excel Project

This project analyzes **11 months of personal banking transactions** using Microsoft Excel to understand income, spending patterns, and net balance over time.

The dataset comes from my own bank exports and has been cleaned, structured, and summarized into an interactive dashboard.

---

## 📂 File Overview

**Main file:**
https://github.com/Pankajr07/Excel--personal-finance-analytics/blob/main/Personal%20Finance%20Project.xlsx

 This is the main workbook containing:
  - raw + cleaned transaction data  
  - category mappings  
  - monthly summaries  
  - PivotTables  
  - an interactive dashboard

**Key Sheets:**

- **`Personal spending`**  
  Core transaction table with:
  - `Date`  
  - `Month-year` (e.g. `2025-01`)  
  - `Unique Id`  
  - `Tran Type` (e.g. EFTPOS)  
  - `Payee` (original description from bank)  
  - `Merchant` (cleaned/standardised name)  
  - `Category` (e.g. Groceries, Dining, Transport, etc.)  
  - `Memo`  
  - `Amount` (negative for spending, positive for income)  
  - `Type` (e.g. `in` / `out`)

  In total, this sheet contains **220 transactions** across **11 months**, grouped into **16 spending categories** and **76 unique merchants**.

- **`MerchantMapping`**  
  Mapping table to clean and standardise merchant names from messy bank descriptions into consistent merchant labels used in the analysis.

- **`Category by month Year`**  
  Aggregated table that summarises total spending per **category per month**, used as the source for charts and dashboard visuals.

- **`Pivot Tables`**  
  A collection of PivotTables used to:
  - calculate total income and total spending  
  - break down spending by category  
  - rank merchants by total spend  
  - summarise monthly trends  

- **`Income Sparklines`**  
  Visual mini-charts to quickly compare income and spending patterns over time.

- **`Dashboard`**  
  The main dashboard view displaying:
  - high-level KPIs  
  - charts for monthly trends and category breakdown  
  - a compact summary of personal finances over the period.

---

## 📊 Metrics & Insights

Using this workbook, I built a dashboard that highlights:

- **Total Income:** 7,126.90  
- **Total Spending:** 6,133.86  
- **Net Balance:** 993.04 (income – spending over the period)

Examples of questions the dashboard can answer:

- Which months had the highest spending?
- Which categories do I spend the most on (e.g. Groceries, Dining, Entertainment)?
- Which merchants receive most of my money over time?
- How does my spending compare month-to-month?

---

## 🧹 Data Cleaning & Preparation

Key data preparation steps in Excel:

1. **Imported bank exports** into the `Personal spending` sheet.
2. Created a `Month-year` column to support monthly summaries and charts.
3. Standardised merchant names using the `MerchantMapping` sheet.
4. Assigned each transaction to a **spending category** (e.g. Groceries, Dining, Shopping, Subscriptions, Transport, etc.).
5. Ensured all amounts were correctly signed (negative for spending, positive for income).
6. Built a structured table ready for PivotTables and dashboarding.

---

## 🛠 Excel Techniques Used

- Structured Tables for transaction data  
- **PivotTables** for aggregation (by month, category, merchant)  
- `SUMIFS`, basic formulas, and calculated fields  
- Custom date grouping (`Month-year`)  
- Dashboard layout using:
  - charts (column/line/donut)  
  - summary cells  
  - references to PivotTable outputs  

---

## 🚀 Future Improvements

- Export the cleaned transaction data into **SQL Server** and replicate the analysis in SQL.
- Build a **Power BI** dashboard on top of the same data model.
- Add more advanced metrics:
  - savings rate %  
  - category-based trend lines  
  - month-over-month % change in key categories.

---

## 🎯 Purpose

This project is part of my analytics portfolio as an **aspiring Data / Reporting Analyst**.

It demonstrates my ability to:
- work with real financial transaction data  
- clean and structure messy exports into usable tables  
- summarise and visualise key metrics in Excel  
- extract practical insights about spending behaviour.
