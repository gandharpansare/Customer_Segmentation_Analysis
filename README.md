# **Customer Segmentation Analysis** 

## **Overview**
This project aims to segment customers based on their **purchasing behaviors, income levels, and engagement with marketing channels** using the **Customer Personality Dataset from Kaggle**. The study applies **Exploratory Data Analysis (EDA), Principal Component Analysis (PCA), Generalized Additive Models (GAMs), and K-means clustering** to identify distinct customer groups. The insights gained from this segmentation can help businesses optimize their **marketing strategies, product offerings, and customer engagement approaches**.

---

## **Dataset**
- **Source**: [Kaggle Customer Personality Analysis](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis/data)
- **Size**: 2,240 observations, 29 variables.
- **Key Features**:
  - **Age**: Customer's age in years.
  - **Income**: Annual household income (USD).
  - **Marital Status**: Single, Widow, Divorced, Couple.
  - **Total Amount Spent**: Customer expenditure across multiple product categories (Fruits, Wines, Meat, Fish, Sweets, Gold).
  - **Purchasing Channels**: Web, Store, Deals, and Catalog.

---

## **Key Research Questions**
1. **Spending vs. Income Across Age Groups**  
   - How does spending behavior vary with increasing income at different life stages?  
   - Are there age-based patterns that affect purchasing decisions beyond income?  

2. **Spending vs. Income Across Marital Status**  
   - Does marital status impact spending behavior relative to income?  
   - Do couples, single customers, and widows follow distinct spending patterns?  

3. **Customer Segmentation**  
   - How can we effectively **group customers based on spending habits and demographics**?  
   - What unique characteristics define each **customer segment**?  

---

## **Methodology**
### **1. Data Preprocessing**
- Handled missing values and outliers.
- Transformed and summarized key variables for a nuanced understanding of customer demographics and purchasing patterns.

### **2. Statistical Modeling**
- **Loess Regression (Degree 2, Span 1)** to analyze spending-income trends.
- **Generalized Additive Models (GAMs)** to capture complex relationships.
- **R-Squared Evaluation** to measure model fit.

### **3. Customer Segmentation using PCA & K-Means Clustering**
- **Principal Component Analysis (PCA)**:
  - PC1 explained **35.8% variance** (strongest influence on spending behaviors).
  - PC2 explained **11.2% variance** (captured engagement with marketing channels).
- **K-Means Clustering (K=3)**:
  - Used **Elbow Method** to determine the optimal number of clusters.
  - Grouped customers into **three distinct segments**.

---

## **Key Findings**
### **1. Spending vs. Income by Age Group**
- **Young Customers (≤35 years)**: Spend conservatively, regardless of income. Their spending is influenced by factors other than income, such as financial responsibility or saving habits.  
- **Mid-Age Customers (36-45 years)**: Show a **sharp increase in spending as income rises**, making them a key target for income-driven marketing.  
- **Older Customers (66-75 years)**: Spending levels off at higher incomes, likely due to **retirement budgeting and reduced expenditure habits**.

### **2. Spending vs. Income by Marital Status**
- **Marital status does not significantly alter the relationship between income and spending.**  
- The GAM model shows that spending trends are **consistent across all marital statuses**, suggesting that **income is the primary factor influencing expenditure**.

### **3. Customer Segmentation Results**
#### **Cluster 1: Emerging Economicals** 
- **Income**: Lowest income bracket, indicating limited spending power.
- **Age**: Younger customers (median age: **41**), newly associated with the company.
- **Digital Engagement**: Highest website visit frequency but **lowest overall spending**.
- **Shopping Behavior**: Price-conscious shoppers who browse frequently but purchase cautiously.
- **Segmentation Label**: **"Emerging Economicals"** or **"Conservative Shoppers"**.

#### **Cluster 2: Established Balancers** 
- **Income**: Middle-income customers with **moderate spending potential**.
- **Age**: Median age **50**, indicating financial stability.
- **Loyalty**: Longest customer tenure, showing **consistent brand engagement**.
- **Shopping Habits**: Balanced spending across all product categories.
- **Engagement**: Regular website visits and purchases via **multiple channels (web, store, deals)**.
- **Segmentation Label**: **"Established Balancers"** or **"Balanced Value Seekers"**.

#### **Cluster 3: High-Income Enthusiasts** 
- **Income**: Highest-income segment.
- **Age**: Median age **45**, representing established professionals.
- **Spending Behavior**: Highest total spending, especially on **wines and meat**.
- **Price Sensitivity**: Least influenced by discounts and promotions.
- **Purchasing Channels**: Engage with online content but prefer in-store purchases.
- **Segmentation Label**: **"High-Income Enthusiasts"** or **"Affluent Explorers"**.

---

## **Strategic Business Implications**
- **High-Income Enthusiasts**: Focus on **premium product offerings** and **exclusive brand experiences**.  
- **Established Balancers**: Implement **personalized loyalty programs** to maintain engagement.  
- **Emerging Economicals**: Improve **website experience, targeted discounts, and promotions** to convert online engagement into purchases.  

---

## **Technologies Used**
- **Programming Language**: R
- **Data Visualization**: ggplot2, PCA scatter plots, GAM trend plots
- **Statistical Modeling**: Loess Regression, Generalized Additive Models (GAMs)
- **Clustering Methods**: Principal Component Analysis (PCA), K-Means Clustering
- **Data Wrangling**: dplyr, tidyr

---

## **Contributors**
- Gandhar Ravindra Pansare
- Swarn Gaba
- Gayatri Gattani
- Rishikesh Kakde
