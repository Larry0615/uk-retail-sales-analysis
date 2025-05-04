# 🛍️ UK Retail Sales Analysis

---

## 📌 Project Overview

This project analyzes over 540,000 historical transactions from a UK-based online retailer.  
The goal is to uncover customer behavior, product performance, and revenue concentration through RFM segmentation and Pareto analysis, enabling data-driven business decisions.

---

## 🔍 Business Problem

The company seeks to answer:
- 🛍️ What products generate the most revenue?
- 📆 What months or seasons perform best in sales?
- 👤 Which customer segments are most valuable?
- 🌍 Are there regional sales trends they can optimize?
- 💰 Is most of the revenue driven by a small set of customers?

---

## 🛠️ Tools & Technologies

- Python (pandas, numpy, matplotlib, seaborn)
- Jupyter Notebook
- SQL (optional queries for deeper exploration)
- Tableau (optional dashboard development)
- Git & GitHub (version control)

---

## 📊 Project Workflow

### 🔗 Data Source:
- UCI Machine Learning Repository – [Online Retail Dataset](https://archive.ics.uci.edu/dataset/352/online+retail)
- Covers one year of UK-based e-commerce transactions (Dec 2010 – Dec 2011)

---

### 🧼 Data Cleaning & Preparation:

- Removed missing values and null customer IDs
- Filtered out canceled transactions (negative quantities)
- Created new column: `SalesRevenue = Quantity × UnitPrice`
- Converted and parsed `InvoiceDate` to datetime format

---

### 📈 Exploratory Data Analysis (EDA):

- Top 10 products by quantity sold
- Monthly revenue trends (peak in Nov & Dec)
- Country-wise revenue analysis (excluding UK)
- Top 10 customers by revenue

---

### 🧠 RFM Customer Segmentation:

Using **Recency, Frequency, and Monetary** scoring:
- Customers scored 1–5 on each metric
- Created a combined RFM segment (e.g., `545`, `112`)
- Labeled segments as:  
  - 🎯 VIP  
  - 💎 Loyal  
  - 🕵️‍♂️ Potential Loyalist  
  - ⚠️ At Risk  
  - ❌ Lost

---

### 📉 Pareto Analysis (80/20 Rule):

- Ranked customers by revenue
- Found that **~22% of customers account for ~80% of total revenue**
- Visualized using a **Pareto curve**
- Confirmed strong **revenue concentration risk** and top-customer dependency

---

### 📊 Visualizations Created:

- Bar chart: Top 10 best-selling products
- Line plot: Monthly sales revenue
- Bar + Pie charts: RFM segment distribution
- Bar chart: Top revenue-generating customers
- Pareto curve: Revenue concentration vs. customer base

---

## 📂 Repository Structure

