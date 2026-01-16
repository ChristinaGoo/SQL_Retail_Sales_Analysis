
# Retail Sales Analysis (PostgreSQL)

## Project Overview
This project analyzes retail transaction data using **PostgreSQL** to uncover sales performance, customer behavior, and operational patterns.  
The analysis focuses on data cleaning, exploratory analysis, and answering business-driven questions using SQL.

Key objectives:
- Validate and clean raw transactional data
- Analyze sales and customer trends
- Identify high-performing categories, customers, and time periods

---

## Dataset & Structure
- **Rows:** 2,000 transactions  
- **Columns:** 11  
- **Time Period:** 2022–2023  
- **Product Categories:** Electronics, Clothing, Beauty  

### Table: `retail_sales`

| Column | Description |
|------|------------|
| transactions_id | Unique transaction identifier |
| sale_date | Date of transaction |
| sale_time | Time of transaction |
| customer_id | Unique customer identifier |
| gender | Customer gender |
| age | Customer age |
| category | Product category |
| quantity | Units sold |
| price_per_unit | Price per unit |
| cogs | Cost of goods sold |
| total_sale | Total transaction value |

### Data Quality Checks
- Missing rows removed: **13 (0.7%)**
- Duplicate rows: **0**
- Final dataset is clean and analysis-ready

---

## Key Insights

### Overall Performance
- **Total Transactions:** 2,000  
- **Unique Customers:** 155  
- **Categories:** 3  

### Revenue by Category
| Category | Total Revenue | Total Orders |
|--------|---------------|--------------|
| Electronics | 313,810 | 684 |
| Clothing | 311,070 | 702 |
| Beauty | 286,840 | 614 |

**Insight:** Electronics generates the highest revenue, while Clothing has the highest transaction volume.

---

### Customer Insights
- **Average customer age (Beauty):** 40.4 years  
- **High-value transactions (> 1,000):** 404  
- **Top 5 customers contribute a disproportionate share of revenue**, indicating revenue concentration among high-value buyers.

---

### Gender & Category Trends
- Transactions are relatively balanced across genders.
- Female customers slightly dominate Beauty purchases.
- Male customers show marginally higher activity in Electronics.

---

### Time-Based Analysis
- **Best-selling months (by average sale):**
  - July 2022
  - February 2023
- **Orders by time of day:**
  - Evening: 1,062
  - Morning: 561
  - Afternoon: 377

**Insight:** Evening hours represent peak purchasing activity, making them ideal for targeted promotions.

---

## SQL Techniques Used
- Data cleaning and validation
- Aggregations and grouping
- Window functions (`RANK()`)
- Common Table Expressions (CTEs)
- Date and time-based analysis

---

## Tools & Technologies
- PostgreSQL
- SQL

---

## Potential Enhancements
- Profitability analysis using COGS
- Customer segmentation (RFM)
- Trend visualization with BI tools or Python
- Seasonal demand forecasting
