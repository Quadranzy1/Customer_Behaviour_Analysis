# 🛍️ Customer Behavior Data Analyst Portfolio Project
This project represents a complete, industry standard, end-to-end data analytics workflow, designed to mirror the real responsibilities of professional analysts in modern business environments. The project encompasses all critical stages of data analysis, from data preparation and modeling to insight generation, visualization, and reporting.

![Python](https://img.shields.io/badge/Python-3.9+-blue?style=for-the-badge&logo=python)
![SQL](https://img.shields.io/badge/MySQL-8.0-orange?style=for-the-badge&logo=mysql)
![Power BI](https://img.shields.io/badge/Power_BI-Dashboard-yellow?style=for-the-badge&logo=powerbi)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas)

## 📖 Project Overview
The goal of this project is to simulate a corporate-grade end-to-end data analytics workflow, demonstrating the ability to translate raw data into strategic business intelligence by:

✅ Data Preparation and Modeling (Python): Clean and transform the raw dataset for analysis.

✅ Data Analysis (SQL): Simulate business transactions, and run queries to extract insights on customer segments, loyalty, and purchase drivers.

✅ Visualization & Insights (Power BI): Build an interactive dashboard that highlights key patterns and trends, enabling stakeholders to make data-driven decisions.

✅ Report and Presentation: Write a clear project report summarizing your key findings and business recommendations. Prepare a presentation that visually communicates insights and actionable recommendations to stakeholders.
---

![Project Workflow](https://github.com/user-attachments/assets/8bbd5dc9-eb6c-40c1-8f19-c08b4107f654)

## 📂 Table of Contents
- [Business Problem](#-business-problem)
- [Data Source](#-data-source)
- [Tech Stack](#-%EF%B8%8F-tech-stack)
- [Methodology](#-methodology)
- [Key Insights](#-key-insights)
- [Recommendations](#-recommendations)
- [Project Structure](#-project-structure)

---

## ❓ Business Problem
A retail company noticed shifts in purchasing patterns across demographics and wanted to leverage their data to answer:
1.  **Who are the most profitable customers?** (Age, Gender, Location)
2.  **Does the subscription model actually increase revenue?**
3.  **Which products drive customer satisfaction and retention?**
4.  **How can we better segment our customers for targeted marketing?**

---

## 💾 Data Source
The dataset consists of **3,900 records** with 18 columns, including:
- **Demographics:** Age, Gender, Location
- **Product Info:** Category, Item Purchased, Size, Color
- **Transaction Info:** Purchase Amount (USD), Payment Method, Shipping Type
- **Status:** Subscription Status, Discount Applied, Frequency of Purchases

---

## 🛠️ Tech Stack
| Tool | Purpose |
| :--- | :--- |
| **Python (Pandas)** | Data cleaning, null value handling, and feature engineering. |
| **SQLAlchemy** | Establishing connection between Python and MySQL database. |
| **MySQL** | Executing complex queries to answer specific business questions. |
| **Power BI** | Creating interactive dashboards to visualize the insights. |

---

## 🔍 Methodology

### 1. Data Cleaning & Feature Engineering (Python)
- **Null Handling:** Imputed missing `Review Rating` values using the median rating of the respective product `Category`.
- **Standardization:** Renamed columns to `snake_case` for SQL compatibility.
- **Feature Engineering:**
    - Created `age_group` bins (*Young Adult, Adult, Middle-aged, Old*).
    - Converted text-based frequencies (e.g., "Weekly") into numeric `purchase_frequency_days`.

### 2. Exploratory Data Analysis (SQL)
Loaded the cleaned data into MySQL to answer 10 specific business questions, such as:
- Calculating revenue contribution by Gender and Age.
- Analyzing the correlation between subscriptions and spending.
- Identifying "Hero Products" based on high review ratings.
- Segmenting customers into **New**, **Returning**, and **Loyal**.

---

## 📊 Key Insights

### 1. 💰 The Gender Revenue Gap
Male customers generate **more than double ($157k)** the revenue of female customers ($75k). The product mix or marketing strategy appears heavily skewed toward men.

### 2. 📉 The Subscription Paradox
Subscribers do **not** spend more per transaction than non-subscribers.
- **Subscriber Avg Spend:** $59.49
- **Non-Subscriber Avg Spend:** $59.87
*Current subscriptions drive frequency, but not basket size.*

### 3. 🏆 High Customer Loyalty
**80%** of the customer base falls into the "Loyal" segment (>10 purchases). While retention is excellent, new customer acquisition is low.

### 4. 👥 Age Demographics
**Young Adults** and **Middle-Aged** customers are the top revenue contributors. The "Old" demographic contributes the least.

### 5. ⭐ Hero Products
The items with the highest customer satisfaction (Review Ratings) are **Gloves (3.86)** and **Sandals (3.84)**.

---

## 💡 Recommendations
- Boost Subscriptions – Promote exclusive benefits for subscribers.
- Customer Loyalty Programs – Reward repeat buyers to move them into the “Loyal” segment.
- Review Discount Policy – Balance sales boosts with margin control.
- Product Positioning – Highlight top-rated and best-selling products in campaigns.
- Targeted Marketing – Focus efforts on high-revenue age groups and express-shipping users.
---

## 📜 License

MIT — feel free to fork, star, and use in your portfolio.

## 👨‍💻 About the Author
Hey, I’m Adediran Quadri, a Data Analyst & Economics Tutor.


## 📁 Project Structure
```bash
├── data/
│   └── customer_shopping_behavior.csv    # Raw dataset
├── notebooks/
│   └── Data_Cleaning_Analysis.ipynb      # Python data prep & feature engineering
├── sql/
│   └── customer_behavior_queries.sql     # SQL scripts for analysis
├── dashboard/
│   └── Shopping_Behavior_Dashboard.pbix  # Power BI Dashboard file
├── presentation/
│   └── Insights_Presentation.pptx        # Final Stakeholder Presentation (PPT)
├── docs/
│   ├── Business_Problem.pdf              # Original Problem Statement & Requirements
│   └── Analysis_Report.pdf               # Detailed Written Report
└── README.md                             # Project documentation



## 💡Thanks for checking out the project! Your support means a lot! Feel free to star ⭐ this repo or share it with someone learning Data Analytics.🚀
