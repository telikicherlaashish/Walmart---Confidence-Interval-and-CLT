# Walmart---Confidence-Interval-and-CLT
Analyzed Walmart Black Friday purchase data to study spending behavior across gender, age, and marital status. Applied EDA, Central Limit Theorem, and confidence interval analysis to compare spending patterns. Generated insights to help Walmart understand customer segments and improve marketing strategies.

# Walmart Customer Purchase Behavior Analysis

## Project Overview

Walmart is one of the largest retail corporations in the world, serving over **100 million customers globally**. During major sales events like **Black Friday**, millions of transactions occur across Walmart stores.

This project analyzes **customer purchase behavior during Black Friday**, focusing on differences in spending patterns across **gender, age groups, and marital status**. The goal is to generate insights that help Walmart better understand its customers and improve business decisions.

The analysis uses **exploratory data analysis (EDA), statistical techniques, and confidence interval estimation based on the Central Limit Theorem (CLT)** to evaluate spending patterns.

---

## Business Problem

The management team at Walmart wants to understand **whether spending habits differ between male and female customers** during Black Friday.

Key questions include:

- Do **women spend more than men** during Black Friday sales?
- What is the **average purchase amount for male vs female customers**?
- Does **marital status influence purchasing behavior**?
- How do **different age groups spend during Black Friday**?
- Can we estimate the **population mean purchase amount using sample data**?

The goal is to use **statistical analysis to estimate spending behavior across 100 million customers (50M male, 50M female).**

---

## Dataset Description

The dataset contains **transaction-level data from Walmart Black Friday sales.**

| Column | Description |
|------|-------------|
| User_ID | Unique customer identifier |
| Product_ID | Product identifier |
| Gender | Customer gender (Male / Female) |
| Age | Age group of the customer |
| Occupation | Occupation category (masked) |
| City_Category | City type (A, B, C) |
| StayInCurrentCityYears | Years spent in current city |
| Marital_Status | 0 = Unmarried, 1 = Married |
| ProductCategory | Product category (masked) |
| Purchase | Purchase amount |

---

## Project Objectives

This analysis aims to:

- Compare **spending behavior between male and female customers**
- Analyze how **age and marital status influence spending**
- Estimate **population mean purchase using sample data**
- Apply the **Central Limit Theorem to study the distribution of sample means**
- Construct **confidence intervals for customer spending**
- Provide **business insights and recommendations**

---

## Data Analysis Steps

### 1. Data Understanding

- Import the dataset
- Check dataset shape and structure
- Inspect data types
- Generate statistical summaries

---

### 2. Data Cleaning

Steps performed:

- Detect missing values using `isnull()`
- Handle missing values if present
- Identify potential outliers using:
  - Boxplots
  - Comparison of mean vs median
  - Descriptive statistics

---

### 3. Exploratory Data Analysis (EDA)

EDA was performed to understand **spending patterns and customer characteristics.**

### Univariate Analysis

Used to study individual variables.

Techniques used:

- Histograms
- Countplots
- Distribution plots

Variables analyzed:

- Gender distribution
- Age groups
- Purchase amount distribution
- City categories

---

### Bivariate Analysis

Used to analyze relationships between variables.

Plots used:

- Boxplots
- Countplots
- Grouped bar charts

Relationships analyzed:

- Gender vs Purchase
- Age vs Purchase
- Marital Status vs Purchase
- City Category vs Purchase

---

### Outlier Detection

Outliers were identified using:

- Boxplots
- Descriptive statistics
- Comparison of mean and median values

The main variable analyzed for outliers was:

- **Purchase amount**

---

## Statistical Analysis

### Central Limit Theorem (CLT)

The Central Limit Theorem was applied to understand the **distribution of sample means for purchase amounts.**

Steps performed:

1. Sample purchase data for male and female customers.
2. Compute sample means for different sample sizes.
3. Observe how the **distribution approaches normal distribution** as sample size increases.

---

### Confidence Interval Estimation

Confidence intervals were calculated to estimate the **population mean spending** for male and female customers.

Confidence levels tested:

- **90% Confidence Interval**
- **95% Confidence Interval**
- **99% Confidence Interval**

These intervals help estimate **the range in which the average spending of 50 million customers is likely to fall.**

---

## Key Insights

Some important findings from the analysis include:

- Male customers generally show **higher average purchase amounts** than female customers during Black Friday.
- The **confidence intervals for male and female spending overlap**, suggesting spending differences are not extremely large.
- Customers aged **26–35 contribute significantly to overall spending.**
- Married customers tend to show **slightly higher spending behavior** compared to unmarried customers.
- City category **B and C customers represent a large share of transactions.**

---

## Business Insights

Based on the analysis:

1. Both male and female customers are important contributors to Black Friday sales.

2. The **26–35 age group represents a high-value customer segment.**

3. Married customers may have **higher household spending power**, influencing their purchase amounts.

4. Confidence interval analysis helps Walmart **estimate spending behavior at the population level.**

---

## Recommendations

Based on the insights, the following recommendations can help Walmart improve business performance:

1. Design **targeted promotions for high-spending age groups such as 26–35 years.**

2. Create **gender-specific marketing campaigns** based on purchasing patterns.

3. Offer **bundle deals or family-oriented promotions** for married customers.

4. Focus on **high-demand product categories during Black Friday promotions.**

5. Use **data-driven marketing strategies** to personalize offers and improve customer engagement.

---

## Tools and Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Jupyter Notebook / Google Colab

---

## Conclusion

This project demonstrates how **exploratory data analysis and statistical techniques such as the Central Limit Theorem and confidence intervals** can be used to analyze large-scale retail data.

The insights generated from this analysis can help Walmart **better understand customer behavior, improve marketing strategies, and make data-driven business decisions during major sales events like Black Friday.**
