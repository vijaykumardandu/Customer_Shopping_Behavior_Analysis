# Customer Shopping Behavior Analysis
### End-to-End Data Analytics Project | Python · MySQL · Power BI

> Analyzed 3,900+ customer transactions to uncover spending patterns, segment customers by loyalty, and deliver a business dashboard with 5 actionable recommendations — using a full analytics stack from raw data to executive-ready insights.

---

## The Business Problem

Retail businesses often sit on large volumes of transactional data with no structured way to answer key questions:

- Which customer segments drive the most revenue?
- Do discounts actually increase spending — or just eat into margins?
- Which products and age groups are worth doubling down on?

This project tackles exactly those questions using a structured, end-to-end analytics workflow.

---

## What I Built

| Layer | Tool | Output |
|---|---|---|
| Data Cleaning & EDA | Python (Pandas, NumPy, Matplotlib, Seaborn) | Clean dataset + exploratory insights |
| Business Queries | MySQL (window functions, CTEs, aggregations) | 10+ stakeholder-ready SQL insights |
| Dashboard | Power BI | Interactive multi-page dashboard |
| Business Report | MS Word | Findings + recommendations document |

---

## Dataset

- **File:** `customer_shopping_behavior.csv`
- **Size:** 3,900 rows × 18 columns
- **Key fields:** Age, Gender, Location, Item Purchased, Category, Purchase Amount, Discount Applied, Subscription Status, Shipping Type, Review Rating, Previous Purchases

**Data quality issue handled:** Missing values in `Review Rating` — imputed using category-wise median to preserve segment accuracy.

---

## Approach

### 1. Data Cleaning (Python)
- Imputed missing `Review Rating` values using **category-wise median** (not global mean — avoids skew across product types)
- Standardized all column names to `snake_case` for SQL compatibility
- Removed redundant columns (`promo_code_used` overlapped with `discount_applied`)
- Engineered two new features: `age_group` (binned age ranges) and `purchase_frequency_tier`

### 2. Exploratory Data Analysis (Python)
- Distribution analysis: age, purchase amount, review ratings
- Spending patterns by product category and gender
- Correlation between discount usage and purchase amount
- Subscription vs non-subscription purchasing behavior
- Visualized using Matplotlib and Seaborn

### 3. SQL Business Analysis (MySQL)
Wrote 10+ advanced queries covering:
- Revenue by customer gender and age group
- Customer segmentation: **New** (1–2 purchases), **Returning** (3–10), **Loyal** (10+) — using window functions
- High-spend customers who used discounts (to separate price-sensitive from brand-loyal buyers)
- Top 5 products by average review rating
- Standard vs. Express shipping spend behavior
- Subscription impact on repeat purchase frequency
- Top items in each category using `RANK()` window function

### 4. Power BI Dashboard
Built an interactive dashboard with:
- Total revenue KPI card
- Revenue by Category, Gender, and Age Group
- Customer Segment breakdown (New / Returning / Loyal)
- Discount usage vs. spend scatter view
- Shipping type revenue comparison
- Dynamic slicers for gender, category, and subscription status

---

## Key Insights

| Finding | Business Implication |
|---|---|
| Loyal customers (10+ purchases) drive the **majority of revenue** | Retention investment has higher ROI than acquisition |
| Express shipping users spend **significantly more per order** | Bundle express shipping with premium products |
| Discount users still spend above average in key categories | Discounts aren't margin killers — they attract high-intent buyers |
| Age group **25–40** is the highest revenue demographic | Target campaigns and promotions here first |
| Top-rated products cluster in **Electronics and Fashion** | Prioritize these in marketing and inventory planning |

---

## Recommendations Delivered

1. **Strengthen loyalty programs** — convert Returning → Loyal customers with milestone rewards
2. **Promote Express Shipping bundles** for high-spend segments to increase average order value
3. **Run targeted promotions** for the 25–40 age group — highest revenue potential
4. **Feature top-rated products** (Electronics, Fashion) prominently in campaigns
5. **Offer subscription-exclusive benefits** to shift Free-tier customers to paid subscriptions

---

## Project Structure

```
Customer_Shopping_Behavior_Analysis/
│
├── customer_shopping_behavior.csv          ← Raw dataset
├── Customer_Shopping_Behavior_Analysis.ipynb  ← Python EDA & cleaning
├── Customer_Shopping_Behavior_Analysis_Queries.sql  ← All MySQL queries
├── Customer_Behavior_dashboard.pbix        ← Power BI dashboard file
├── Customer Shopping Behavior Analysis.docx ← Business report
└── README.md
```

---

## Skills Demonstrated

- **Data preparation & cleansing** — handling missing values, feature engineering, standardization
- **SQL analytics** — window functions, CTEs, customer segmentation, aggregations
- **Data visualization** — interactive Power BI dashboards with KPIs, slicers, and trend analysis
- **Business communication** — translating raw findings into stakeholder-ready insights and recommendations
- **Risk analysis** — identifying high-loss discount segments and low-performing categories

---

## Dashboard Preview
<img width="2011" height="1098" alt="Screenshot 2025-11-16 112647" src="https://github.com/user-attachments/assets/b65da524-750d-48a3-b429-2b4dabcaa0a5" />


