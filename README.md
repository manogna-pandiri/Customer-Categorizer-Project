# 📊 Customer Personality Analysis and Marketing Campaign Prediction

## 📌 Project Overview

This project focuses on analyzing customer demographics, purchasing behavior, and marketing campaign responses to understand customer personalities, identify valuable customer segments, and predict campaign acceptance.

The project combines Exploratory Data Analysis (EDA), Feature Engineering, Customer Segmentation using K-Means Clustering, and Machine Learning Classification Models to generate actionable business insights and improve marketing effectiveness.

The primary goal is to help businesses optimize marketing campaigns, improve customer retention, and increase return on investment (ROI) through data-driven decision-making.

---

## 🎯 Business Problem

Marketing campaigns are often launched without a clear understanding of customer behavior, resulting in:

- Low campaign conversion rates
- Inefficient marketing expenditure
- Poor customer targeting
- Reduced customer engagement

This project aims to solve these challenges by:

- Understanding customer purchasing patterns
- Identifying distinct customer groups
- Predicting campaign acceptance
- Improving marketing strategy through customer segmentation

---

## 📂 Dataset Information

The dataset contains customer demographic information, purchasing history, and campaign response data.

### Key Features

#### Customer Demographics

- Year_Birth
- Education
- Marital_Status
- Income

#### Product Spending

- MntWines
- MntFruits
- MntMeatProducts
- MntFishProducts
- MntSweetProducts
- MntGoldProds

#### Purchase Channels

- NumWebPurchases
- NumCatalogPurchases
- NumStorePurchases

#### Customer Engagement

- NumWebVisitsMonth
- AcceptedCmp1
- AcceptedCmp2
- AcceptedCmp3
- AcceptedCmp4
- AcceptedCmp5
- Response

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Jupyter Notebook
- GitHub

---

## 🔍 Exploratory Data Analysis (EDA)

The EDA phase focused on understanding customer demographics, purchasing behavior, and campaign engagement patterns.

### Analysis Performed

- Data Cleaning
- Missing Value Analysis
- Outlier Detection
- Correlation Analysis
- Distribution Analysis
- Customer Demographic Analysis
- Product Spending Analysis

### Key Findings

### Income vs Spending

Customers with higher income levels tend to spend significantly more across all product categories.

### Product Preference

Wine and Meat Products contribute the highest share of customer spending.

### Customer Demographics

Middle-aged customers represent the largest portion of the customer base.

### Purchase Channels

Store purchases are more frequent than catalog and web purchases.

---

## ⚙️ Feature Engineering

Several new business-focused features were created to improve clustering and classification performance.

### Features Created

### Customer Age

```python
Age = Current_Year - Year_Birth
```

### Total Spending

```python
Total_Spending = (
    MntWines +
    MntFruits +
    MntMeatProducts +
    MntFishProducts +
    MntSweetProducts +
    MntGoldProds
)
```

### Total Purchases

```python
Total_Purchases = (
    NumWebPurchases +
    NumCatalogPurchases +
    NumStorePurchases
)
```

### Family Size

Derived from marital status and household information.

### Customer Tenure

Calculated using enrollment dates.

---

## 🤖 Customer Segmentation using K-Means Clustering

### Objective

Segment customers into distinct groups based on demographic characteristics and purchasing behavior.

### Features Used

- Income
- Age
- Total Spending
- Purchase Frequency
- Family Size

### Clustering Technique

- K-Means Clustering

### Outcome

Customers were grouped into meaningful segments with similar behavioral patterns.

---

## 📈 Customer Segments Identified

### Cluster 0 – High Value Customers

#### Characteristics

- High Income
- High Spending
- Frequent Purchases
- High Customer Value

#### Business Strategy

- Loyalty Programs
- Premium Memberships
- Personalized Recommendations
- Exclusive Offers

---

### Cluster 1 – Moderate Value Customers

#### Characteristics

- Moderate Income
- Average Spending
- Regular Purchasing Activity

#### Business Strategy

- Cross-Selling
- Product Bundling
- Upselling Campaigns

---

### Cluster 2 – Low Engagement Customers

#### Characteristics

- Lower Spending
- Infrequent Purchases
- Low Campaign Engagement

#### Business Strategy

- Re-engagement Campaigns
- Discount Offers
- Retention Programs

---

## 📊 Clustering Insights

### Observation 1

A relatively small customer segment contributes a large share of total revenue.

### Observation 2

High-income customers consistently exhibit higher spending behavior.

### Observation 3

Customer purchase patterns differ significantly across clusters.

### Observation 4

Personalized marketing strategies are more effective than generic campaigns.

---

## 🤖 Predictive Modeling

### Objective

Predict whether a customer is likely to respond positively to a marketing campaign.

### Machine Learning Workflow

1. Data Preprocessing
2. Feature Selection
3. Train-Test Split
4. Model Training
5. Model Evaluation

---

## 🔍 Feature Selection

Feature selection was performed to identify the most influential variables affecting campaign response.

### Important Features

- Income
- Total Spending
- Age
- Purchase Frequency
- Previous Campaign Responses
- Web Purchase Activity

These features showed strong predictive power in determining campaign acceptance.

---

## 🧠 Classification Models

The following machine learning models were evaluated:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier

### Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

## 📌 Key Insights and Observations

### Customer Spending Behavior

Customers with higher income contribute significantly more revenue than lower-income customers.

### Product Preferences

Wine products generate the highest customer spending compared to other product categories.

### Marketing Campaign Performance

Customers who previously accepted campaigns are more likely to respond positively to future campaigns.

### Customer Segmentation

Distinct customer groups exist within the customer base, each requiring different marketing approaches.

### Customer Value Distribution

A small percentage of customers contribute a disproportionately large share of sales revenue.

---

## 💡 Business Recommendations

### 1. Focus on High-Value Customers

Implement loyalty and retention programs for high-spending customers.

### 2. Personalize Marketing Campaigns

Create segment-specific marketing campaigns rather than mass marketing.

### 3. Improve Campaign Targeting

Use predictive models to target customers most likely to respond.

### 4. Increase Customer Lifetime Value

Leverage cross-selling and upselling opportunities for moderate-value customers.

### 5. Re-engage Low Activity Customers

Develop retention campaigns and special offers to increase engagement.

---

## 🚀 Business Benefits

This project provides several business advantages:

### Improved Marketing Efficiency

Targeting the right customers reduces unnecessary marketing costs.

### Higher Campaign Response Rates

Predictive modeling helps identify customers most likely to convert.

### Better Customer Segmentation

Businesses can tailor offers based on customer needs and behavior.

### Increased Revenue

High-value customers can be identified and retained more effectively.

### Enhanced Customer Experience

Personalized campaigns improve customer satisfaction and engagement.

### Data-Driven Decision Making

Business decisions are supported by analytical insights rather than assumptions.

---

## 📁 Repository Structure

```text
Customer-Personality-Analysis/
│
├── marketing_campaign.csv
├── EDA.ipynb
├── Feature_engineering_and_clustering.ipynb
├── Feature_selection_and_classification.ipynb
├── clustered_data.csv
├── clustered_data-checkpoint.csv
└── README.md
```

---

## 🎯 Skills Demonstrated

- Exploratory Data Analysis (EDA)
- Data Cleaning
- Feature Engineering
- Data Visualization
- Customer Segmentation
- K-Means Clustering
- Machine Learning
- Classification Modeling
- Predictive Analytics
- Business Intelligence
- Marketing Analytics
- Python Programming

---

## 👩‍💻 Author

**Manogna**

Aspiring Data Analyst | Business Analyst | Data Science Enthusiast

---

## ⭐ Project Outcome

This project successfully transformed raw customer data into actionable business insights by combining customer segmentation and predictive analytics. The findings can help organizations improve customer targeting, optimize marketing campaigns, increase customer retention, and maximize overall business profitability.
