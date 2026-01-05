# 🛍️ Customer Shopping Behavior Analysis

## 📌 Project Overview
This project analyzes customer shopping behavior using transactional data from **3,900 purchases** across multiple product categories.  
The objective is to uncover insights into **spending patterns, customer segments, product preferences, and subscription behavior** to support strategic, data-driven business decisions.

---

## 📊 Dataset Summary
- **Rows:** 3,900  
- **Columns:** 18  

### Key Features
- **Customer Demographics:** Age, Gender, Location, Subscription Status  
- **Purchase Details:** Item Purchased, Category, Purchase Amount, Season, Size, Color  
- **Shopping Behavior:**  
  Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases,  
  Review Rating, Shipping Type  

### Data Quality
- **Missing Values:** 37 missing entries in the *Review Rating* column  

---

## 🛠️ Tools & Technologies
- **Python:** Pandas, NumPy  
- **SQL:** PostgreSQL  
- **BI Tool:** Power BI  
- **Environment:** Jupyter Notebook  

---

## 🔍 Exploratory Data Analysis (Python)
Data preparation and cleaning were performed using Python:

- **Data Loading:** Imported dataset using Pandas  
- **Initial Exploration:**  
  - `df.info()` for structure  
  - `df.describe()` for summary statistics  
- **Missing Data Handling:**  
  - Imputed missing *Review Rating* values using the **median rating per product category**  
- **Column Standardi**
