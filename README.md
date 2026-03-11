# Customer_Shopping_Behavior_Analysis
This project analyzes customer shopping behavior using real transactional data.
The goal is to understand spending patterns, product preferences, customer segments, discount usage, and subscription behavior through:

1. Python-based data cleaning & exploratory analysis

2. MySQL queries for business insights

3. Interactive Power BI dashboards

4. Final business report & presentation

5. This project demonstrates a complete end-to-end data analytics workflow, from raw data → insights → dashboard → recommendations.

## Dataset

File: customer_shopping_behavior.csv
Rows: 3,900
Columns: 18

Key Features

1. Demographics: Age, Gender, Location, Subscription Status

2. Shopping Data: Item Purchased, Category, Purchase Amount

3. Behavioral Data: Discount Applied, Previous Purchases, Frequency

4. Product Details: Size, Color, Shipping Type, Review Rating

5. Missing Values: Present in the Review Rating column

## Tools & Technologies

| Purpose                    | Tools                        |
| -------------------------- | ---------------------------- |
| Data Loading & Cleaning    | Python, Pandas, NumPy        |
| EDA & Visualization        | Python (Matplotlib, Seaborn) |
| Database & SQL Queries     | MySQL                        |
| Dashboard                  | Power BI                     |
| Report Writing             | MS Word                      |
| Presentation               | Gamma App                    |
| Version Control (optional) | Git & GitHub                 |


## Project Steps
1. Load & Explore Data (Python)

- Imported dataset using pandas

- Used df.info(), df.describe(), and visual checks

- Identified missing values and inconsistencies

2. Data Cleaning

- Imputed missing Review Ratings using category-wise median

- Standardized column names to snake_case

- Removed redundant columns (e.g., promo_code_used if overlap with discount_applied)

- Created new features:

- age_group (binned age ranges)

- Purchase frequency metrics

3. Exploratory Data Analysis (EDA)

- Distribution of age, purchase amount, and ratings

- Category-level spend patterns

- Gender-wise and subscription-wise purchasing behavior

- Correlation between discounts and spending

- Visualizations using matplotlib/seaborn

4. SQL Analysis (MySQL)

- Imported the cleaned dataset into MySQL and performed business queries such as:

- Revenue by Customer Gender

- High-spending customers who used discounts

- Top 5 products by average rating

- Standard vs. Express Shipping behavior

- Products with highest discount usage

- Customer Segmentation (New, Returning, Loyal)

- Top items in each category using window functions

- Subscription impact on repeat purchases

- Revenue contribution by age group

5. Power BI Dashboard

- Built an interactive dashboard containing:

- Total Revenue

- Revenue by Category & Gender

- Top Products & Ratings

- Customer Segments

- Discount & Subscription Insights

- Shipping Type Analysis

- Age Group Revenue Trends

6. Business Report

- Prepared a clear, concise report summarizing:

- Findings from Python EDA

- SQL insights

- Dashboard interpretation

- Business recommendations

7. Presentation 

- Created a visually clean slide deck presenting:

- Problem Statement

- Methodology

- Key Insights

- Visuals from SQL & Power BI

- Final Recommendations

## Results & Insights

**Key Insights**

- Female customers generated slightly higher revenue than males.

- Several customers using discounts still spent above average, indicating strong interest in specific product categories.

- Express shipping users tend to make higher-value purchases.

- Top-rated products mainly fall under categories like Electronics and Fashion.

- Loyal customers (>10 purchases) drive the majority of revenue.

- High-revenue age groups: 25–40 years.

**Recommendations**

- Strengthen loyalty programs to convert returning customers into loyal buyers.

- Promote Express Shipping bundles for high-spending segments.

- Highlight top-rated & high-revenue products in marketing campaigns.

- Offer targeted promotions to age groups with strong spending patterns.

- Encourage transition from Free → Subscription with exclusive benefits.

![Dashboard]<img width="2011" height="1098" alt="Screenshot 2025-11-16 112647" src="https://github.com/user-attachments/assets/5971d059-a705-40e7-8a83-6f9668fd2ee0" />

