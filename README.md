# marketing-analytics-portfolio
# Consumer Behavior Analysis & Predictive Modeling

**Author:** Eleni Kaltsouni  
**Focus:** Marketing Analytics, Customer Segmentation, Predictive Modeling  


---

##  Project Overview
In the highly competitive e-commerce landscape, understanding customer behavior is the key to driving revenue and optimizing marketing strategies. The primary objective of this project is to analyze online shoppers' intention and build a classification model that predicts whether a website visitor will make a purchase (Revenue = True/1) or abandon their cart (Revenue = False/0).

This analysis is based on a dataset of **12,330 distinct online shopping sessions**, capturing 18 attributes related to user behavior and contextual information.

##  The Business Problem
*   **High Churn Rates:** Why do visitors leave without purchasing?
*   **Resource Allocation:** How can marketing and CRM teams identify high-intent visitors to target with personalized offers?
*   **Data-Driven Decisions:** Can we predict purchasing intent based on clickstream data (e.g., time spent on product pages, bounce rates, visit timing)?

##  Tools & Technologies Used
*   **Python:** Pandas, NumPy (Data Manipulation)
*   **Scikit-Learn:** Logistic Regression, K-Nearest Neighbors (Machine Learning)
*   **Matplotlib & Seaborn:** Data Visualization

---

##  Methodology & Workflow

### 1. Exploratory Data Analysis (EDA) & Data Cleaning
*   Identified and removed highly correlated features (e.g., dropping `BounceRates` due to high Variance Inflation Factor - VIF) to prevent multicollinearity.
*   Filtered outliers to ensure robust model performance.
*   Analyzed class imbalance in the target variable (`Revenue`).

### 2. Feature Engineering & Preprocessing
*   Converted categorical variables (`Month`, `VisitorType`) into numerical formats using Dummy Encoding.
*   Scaled all features using `StandardScaler` to prepare the data for distance-based algorithms like KNN.

### 3. Predictive Modeling
Trained and evaluated three distinct classification models to establish a performance baseline and optimize predictive accuracy:
1.  **Logistic Regression** (Baseline)
2.  **K-Nearest Neighbors (k=3)**
3.  **K-Nearest Neighbors (k=9)**

---

##  Key Business Insights & Results

Both the Logistic Regression and the optimized KNN (k=9) models achieved an impressive **overall accuracy of 88%**. 

To demonstrate the real-world application of this model, I simulated a hypothetical "New Visitor" entering the site with specific characteristics (e.g., high time spent on product pages, low exit rate, visiting on a weekend). 
*   **The Outcome:** The model successfully predicted a **93% probability of purchase** for this specific visitor profile.

---
*Note: The Jupyter Notebook containing the full Python code, visualizations, and statistical breakdowns is included in this repository.*
