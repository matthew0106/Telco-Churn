# Customer Churn Analysis

![image](https://github.com/user-attachments/assets/2d58a5d8-fc3d-4a3c-9acb-f6ae12befa00)


## Overview
This project analyses customer churn in a telecom dataset to identify key factors influencing churn and develop predictive models for better customer retention strategies.

## Dataset
The dataset includes customer details, usage patterns, and service interactions. Key features:
- **Account Length**
- **Call Minutes** (Day, Evening, Night, International)
- **Number of Calls** (Day, Evening, Night, International)
- **Voicemail & International Plans**
- **Customer Service Calls**
- **Churn Label (Target Variable)**

## Methodology

### 1. Data Import
- The dataset is loaded using **Pandas** for data manipulation.

### 2. Data Cleaning & Preprocessing
- Handling missing values.
- Encoding categorical variables for machine learning compatibility.
- Standardising numerical features to optimize model performance.

### 3. Exploratory Data Analysis (EDA)

#### 3.1 Basic Statistics & Distributions
- Summary statistics to understand feature distributions.

#### 3.2 Churn Analysis
- **Overall churn rate calculation.**
- **Churn distribution by state.**
- **Churn behavior based on voicemail & international plans.**
- **Correlation between customer service calls and churn.**

📌 **Key Findings:**
- **California & New Jersey have the highest churn rates.**
- **40% of customers with international plans churn.**
- **Increased customer service calls correlate with higher churn.**

#### 3.3 Feature Correlations
- Identifying relationships between numerical features & churn.

### 4. Feature Engineering
- Encoding categorical features using **One-Hot Encoding.**
- Standardising numerical variables with **StandardScaler.**
- Creating new features to improve predictive power.

### 5. 🤖 Machine Learning Models & Evaluation

### 📌 Logistic Regression:
- **Accuracy:** 86%
- **Precision:** 
  - **88%** (Non-Churn)
  - **53%** (Churn)
- **Recall:** 
  - **97%** (Non-Churn)
  - **21%** (Churn)
- **Pros:** Simple, interpretable model, less prone to overfitting.

### 📌 Decision Tree Classifier:
- **Accuracy:** 91%
- **Precision:** 
  - **95%** (Non-Churn)
  - **66%** (Churn)
- **Recall:** 
  - **94%** (Non-Churn)
  - **72%** (Churn)
- **Cons:** Prone to overfitting, less generalizable.

✅ **Final Model Selection:**  
**Logistic Regression** was chosen for its **better generalisation and interpretability** over complex models.

---

## 📊 Key Findings & Business Recommendations

### 🔎 **Findings:**
- **Customers with High `CustServ_Calls` & `Intl_Plan` Subscriptions Are More Likely to Churn.**
- **High `Day_Charge` Significantly Impacts Churn Probability.**
- **Frequent Customer Service Calls Indicate Customer Dissatisfaction.**

### 📈 **Recommendations:**
✅ **Improve Customer Support Services:** Reduce dissatisfaction by enhancing **response times and issue resolution**.  
✅ **Offer Competitive International Plans:** Reduce churn by introducing **better international call rates**.  
✅ **Optimise Pricing Strategies for High-Usage Customers:** Provide **discounts or incentives** to retain high-value users.  

---

## 📦 Dependencies
Ensure the following libraries are installed before running the analysis:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn

