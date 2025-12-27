# Customer Shopping Behavior Analysis

## 📌 Overview

This project analyzes transactional data from **3,900 purchases** across various product categories to uncover deep insights into customer spending patterns and preferences. The primary goal is to identify key customer segments, evaluate subscription behavior, and analyze the impact of discounts to guide strategic business decisions.

---

## 📊 Dataset

*  **Source:** Transactional Shopping Data.


*  **Size:** 3,900 rows and 18 columns.


*  **Key Features:** * **Demographics:** Age, Gender, Location, and Subscription Status.


*  **Purchase Details:** Item Purchased, Category, Purchase Amount, and Season.


*  **Behavioral Data:** Review Ratings, Shipping Type, and Purchase Frequency.




*  **Data Quality:** Addressed 37 missing values in the `Review Rating` column.



---

## 🛠 Tools & Technologies

*  **Data Processing:** Python (Pandas).


*  **Database Management:** MSSQL.


*  **Visualization:** Power BI.


* **Reporting & Presentation:** Gamma AI (Presentation) and Markdown (Documentation).

---

## 🚀 Project Steps

### 1. Data Cleaning & Preparation (Python)

*  **Missing Value Imputation:** Filled nulls in `Review Rating` using the median rating per product category.


*  **Standardization:** Converted column names to `snake_case` for consistency.


*  **Feature Engineering:** Created `age_group` bins and a `purchase_frequency_days` column.


*  **Redundancy Check:** Dropped the `promo_code_used` column as it was redundant with `discount_applied`.



### 2. Structured Analysis (SQL)

*  **Revenue Segmentation:** Calculated total revenue by gender and age group.


*  **Behavioral Querying:** Identified high-spending discount users and compared subscriber vs. non-subscriber performance.


*  **Ranking:** Determined the top 3 most-purchased products within every category.



### 3. Interactive Dashboard (Power BI)

* Developed a comprehensive **Customer Behavior Dashboard** visualizing:
* Key KPIs: Total Customers (3.9K), Avg Purchase ($59.76), and Avg Rating (3.75).


* Revenue and Sales distributions by Category and Age Group.


* Subscription split (27% Yes / 73% No).





---

## 📈 Key Results & Insights

*  **Revenue Leaders:** Male customers generated significantly higher revenue (**$157,890**) compared to female customers ($75,191).


*  **Top Age Group:** **Young Adults** are the highest revenue-contributing segment ($62,143).


*  **Customer Loyalty:** The majority of the customer base (**3,116**) is classified as "Loyal".


*  **Product Performance:** **Clothing** is the dominant category in both revenue and total sales.


*  **Shipping Impact:** Customers using Express shipping spend slightly more on average ($60.48) than those using Standard shipping ($58.46).



---

## 💡 Business Recommendations

*  **Subscription Growth:** Promote exclusive benefits to convert the 73% of non-subscribers.


*  **Loyalty Incentives:** Implement rewards for the "Returning" segment to transition them into "Loyal" customers.


*  **Targeted Marketing:** Focus high-tier marketing campaigns on the **Young Adult** demographic and high-revenue categories like **Clothing**.



---

## ⚙️ How to Run

1. **Environment:** Ensure you have Python 3.x and a SQL instance running.
2. **Preprocessing:** Run the `cleaning_script.py` to generate the `cleaned_customer_data.csv`.
3. **SQL Analysis:** Import the cleaned CSV into SQL and execute the scripts in the `/queries` folder.
4. **Visualization:** Open the `Customer_Behavior_Dashboard.pbix` file in Power BI Desktop to interact with the visuals.

---

**Author:** Yusuf Mehmet Arslan
