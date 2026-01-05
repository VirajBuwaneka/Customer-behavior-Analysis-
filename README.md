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
- **Column Standardization:**  
  - Renamed all columns to **snake_case** for consistency  
- **Feature Engineering:**  
  - Created `age_group` by binning customer ages  
  - Created `purchase_frequency_days` from purchase data  
- **Data Consistency Check:**  
  - Verified redundancy between `discount_applied` and `promo_code_used`  
  - Dropped `promo_code_used` column  
- **Database Integration:**  
  - Loaded the cleaned dataset into **PostgreSQL** for SQL-based analysis  

---

## 🧮 Data Analysis Using SQL (Business Transactions)
The following business questions were answered using SQL:

1. Revenue comparison by **gender**  
2. Identification of **high-spending customers who used discounts**  
3. **Top 5 products** by average review rating  
4. Comparison of **average purchase amount** by shipping type (Standard vs Express)  
5. **Subscribers vs Non-Subscribers** revenue and spending comparison  
6. Products with the **highest dependency on discounts**  
7. **Customer segmentation** into New, Returning, and Loyal customers  
8. **Top 3 most purchased products** in each category  
9. Relationship between **repeat purchases (>5)** and subscription likelihood  
10. **Revenue contribution by age group**  

---

## 📈 Dashboard (Power BI)
An interactive **Power BI dashboard** was created to visually present:
- Customer segments  
- Revenue trends  
- Product performance  
- Subscription behavior  

---

## 💡 Business Recommendations
- **Boost Subscriptions:** Promote exclusive benefits to increase conversions  
- **Customer Loyalty Programs:** Reward repeat buyers to build long-term loyalty  
- **Review Discount Policy:** Balance sales growth with profit margins  
- **Product Positioning:** Highlight top-rated and best-selling products  
- **Targeted Marketing:** Focus on high-revenue age groups and express-shipping users  

---

## ✅ Key Takeaways
This project demonstrates an **end-to-end data analytics workflow**, including:
- Data cleaning & feature engineering  
- SQL-driven business analysis  
- Dashboard creation for stakeholders  
- Actionable, data-backed recommendations  

