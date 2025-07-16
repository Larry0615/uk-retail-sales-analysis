#  UK Retail Sales Analysis

---

##  Project Overview

This project analyzes over **540,000 historical transactions** from a UK-based online retailer.  
The goal is to uncover customer behavior, product performance, and revenue concentration through **RFM segmentation** and **Pareto analysis**, enabling data-driven business decisions.

---

##  Business Problem

The company seeks to answer:
-  What products generate the most revenue?
-  What months or seasons perform best in sales?
-  Which customer segments are most valuable?
-  Are there regional sales trends they can optimize?
-  Is most of the revenue driven by a small set of customers?

---

##  Tools & Technologies

- **Python**: `pandas`, `numpy`, `matplotlib`, `seaborn`
- **Jupyter Notebook**
- **SQL** (optional queries for deeper exploration)
- **Tableau** (optional dashboard development)
- **Git & GitHub** (for version control)

---

##  Project Workflow

###  Data Source
- UCI Machine Learning Repository – [Online Retail Dataset](https://archive.ics.uci.edu/dataset/352/online+retail)
- Covers one year of UK-based e-commerce transactions (Dec 2010 – Dec 2011)

---

###  Data Cleaning & Preparation

- Removed missing values and null `CustomerID`s
- Filtered out canceled transactions (negative quantities)
- Created new column: `SalesRevenue = Quantity × UnitPrice`
- Parsed `InvoiceDate` to datetime format

---

###  Exploratory Data Analysis (EDA)

- Top 10 products by quantity sold
- Monthly revenue trends (peaks in Nov & Dec)
- Country-wise revenue analysis (excluding UK)
- Top 10 customers by total revenue

---

###  RFM Customer Segmentation

Using **Recency**, **Frequency**, and **Monetary** scoring:
- Customers scored from 1–5 on each metric
- Combined into RFM Segment Codes (e.g., `545`, `112`)
- Segments labeled as:
  - 🎯 VIP  
  - 💎 Loyal  
  - 🕵️‍♂️ Potential Loyalist  
  - ⚠️ At Risk  
  - ❌ Lost

---

###  Pareto Analysis (80/20 Rule)

- Ranked customers by total revenue
- Found that **~22% of customers account for ~80% of total revenue**
- Visualized using a Pareto curve
- Confirmed strong revenue concentration and top-customer dependency

---
##  Key Findings

- 🛍️ **Top-selling product**: WORLD WAR 2 GLIDERS ASSTD DESIGNS  
- 💰 **Top customer** generated over £279,000 in revenue  
- 🌍 **Top countries** (excluding UK): Netherlands, EIRE, Germany  
- 📆 **Peak sales months**: November and December  
- 📊 **RFM Segment distribution**:
  - 25.5% Potential Loyalists  
  - 22.7% Loyal  
  - 21.7% VIP  
  - 17.9% At Risk  
  - 12.3% Lost  
- 📉 **Pareto Insight**: ~22% of customers drive ~80% of total revenue

---

##  Business Recommendations

-  Focus on retaining **VIP and Loyal** customers through personalized engagement
-  Launch **win-back campaigns** for **At Risk** customers
-  Expand marketing in top-performing international countries
-  Prepare for **Q4 sales peaks** with increased inventory and targeted promotions
-  Use RFM segmentation for **email marketing and personalization**

---
## 📊 Visualizations Created

-  Bar chart: Top 10 best-selling products  
-  Line plot: Monthly sales revenue  
-  Bar & Pie charts: RFM segment distribution  
-  Bar chart: Top customers by revenue  
-  Pareto curve: Revenue concentration vs. customer base

---
## 📂 Repository Structure
```
uk-retail-sales-analysis/
│
├── data/
│ └── raw/ ← Original dataset
│
├── notebooks/
│ └── uk_retail_analysis.ipynb ← Jupyter notebook with full analysis
│
├── visuals/
│ ├── top_10_products.png
│ ├── monthly_sales.png
│ ├── customer_segments_bar.png
│ ├── customer_segments_pie.png
│ └── pareto_chart.png
│
└── README.md
```
---

## 🚀 Future Work (Optional)

- 📊 Develop an interactive **Tableau dashboard**
- 🔮 Build a **predictive CLV (Customer Lifetime Value)** model
- 🧠 Automate RFM segmentation using reusable functions or classes

---

📬 **Let’s connect**  
Want to collaborate or give feedback?  
Check out more of my work at: [github.com/Larry0615](https://github.com/Larry0615)

