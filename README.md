# 🛍️ UK Retail Sales Analysis

---

## 📌 Project Overview

This project analyzes over 540,000 retail transactions from a UK-based online retailer.  
The goal is to uncover sales trends, identify high-value customer segments using RFM analysis, and assess revenue concentration using Pareto analysis to support strategic decision-making.

---

## 🔍 Business Objectives

The company wants to understand:
- 📦 What products generate the most revenue?
- 📅 What months or seasons perform best in sales?
- 👤 Which customer segments are most valuable?
- 🌍 Are there regional sales trends they can optimize?

---

## 🛠️ Tools & Technologies Used

- Python: pandas, NumPy, matplotlib, seaborn
- SQL (optional queries)
- Tableau (for interactive dashboard)
- Excel / Google Sheets (supporting calculations)
- Jupyter Notebook + Git + GitHub (for version control)

---

## 📊 Project Workflow

### 1. 🔍 Data Source
- [Online Retail Dataset – UCI Repository](https://archive.ics.uci.edu/dataset/352/online+retail)
- One year of e-commerce transactions from 2010–2011

### 2. 🧼 Data Cleaning
- Removed nulls and canceled invoices
- Created new metrics (e.g., `SalesRevenue = Quantity * UnitPrice`)
- Converted dates, handled customer IDs

### 3. 📈 Exploratory Data Analysis
- Top 10 best-selling products by quantity
- Monthly revenue trends 
- Top countries outside the UK by sales revenue
- Top 10 customers by revenue

### 4. 📊 RFM Segmentation
- **Recency, Frequency, Monetary** scores (1–5 scale)
- Segmented customers into: 🎯 VIP, 💎 Loyal, 🔁 Potential Loyalist,
  ⚠️ At Risk, and ❌ Lost.

### 5. 📉 Pareto Analysis (Bonus Insight)
- Confirmed **~22% of customers account for ~80% of total revenue**
- Revealed high revenue concentration
- Business implication: prioritize VIP and Loyal segments

---

## 📈 Key Findings

- 🛍️ **Top-selling product**: "WORLD WAR 2 GLIDERS ASSTD DESIGNS"
- 💰 **Top customer** generated over £279,000 in revenue
- 🌍 **Top countries** outside UK: Netherlands, EIRE, Germany
- 📆 **Peak sales months**: November and December
- 🧠 **Pareto insight**: ~22% of customers contribute 80% of sales
- 📊 **Segment share**:
  - 25.5% Potential Loyalists
  - 22.7% Loyal
  - 21.7% VIP
  - 17.9% At Risk
  - 12.3% Lost

---

## 📢 Business Recommendations

- 🎯 Prioritize top 20–25% of customers (VIPs & Loyal) with loyalty programs and personalized campaigns
- 🧪 A/B test email or seasonal offers targeting “At Risk” group to reduce churn
- 🌍 Expand campaigns in high-performing countries like the Netherlands and EIRE
- 📆 Leverage seasonal peaks in Q4 (especially Nov/Dec) with inventory and promotions

---

## 📂 Repository Structure

