# Customer Activity Analysis and Forecasting for "One Click" Online Store

This project is dedicated to developing a customer activity prediction system for the **"One Click"** online store.

## Project Goal

To create a machine learning model that helps the online store **retain regular customers** by analyzing behavioral and financial data.

---

## Project Objectives

- Build a model that predicts the **probability of decreased customer activity** in the next 3 months;
- Segment customers based on model predictions and customer profitability;
- Provide **actionable recommendations** to increase customer engagement for the most critical segment.

---

## Project Plan

### 1. Data Overview
- Load and examine data from multiple sources;
- Ensure consistency between the tables and their descriptions.

### 2. Data Preprocessing
- Handle missing values, duplicates, and incorrect entries.

### 3. Exploratory Data Analysis (EDA)
- Analyze distributions of key metrics;
- Select customers active in the past 3 months.

### 4. Data Merging
- Combine all relevant tables into one modeling dataset;
- Split data into historical and current periods.

### 5. Correlation Analysis
- Investigate relationships between features;
- Handle multicollinearity if necessary.

### 6. Modeling
- Prepare data with encoding and scaling;
- Train and tune models:
  - `KNeighborsClassifier`
  - `DecisionTreeClassifier`
  - `LogisticRegression`
  - `SVC`
- Select the best model based on ROC-AUC score.

### 7. Feature Importance
- Use SHAP to interpret the best model;
- Identify key drivers of customer activity decline.

### 8. Customer Segmentation
- Segment customers using prediction and profitability;
- Develop personalized strategies for retention.

### 9. Final Summary
- Summarize results and conclusions;
- Highlight critical insights and business recommendations.

---

## Data Description

| File             | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| `market_file.csv` | Customer behavior, marketing interactions, purchase preferences            |
| `market_money.csv`| Revenue information for different periods                                  |
| `market_time.csv` | Time spent on the website                                                   |
| `money.csv`       | Customer profit for the last three months                                   |

---

## Final Results

### Project Summary

The project aimed to **predict customer activity decline** and provide strategies to boost engagement through data-driven segmentation.

### Data and Preprocessing

- Customer activity metrics, revenue, time on site, and other features were analyzed;
- Preprocessing included:
  - Standardizing text fields;
  - Fixing typos;
  - Keeping outliers for analysis;
  - Merging datasets for modeling.

### Model Selection

- Models trained: `KNeighborsClassifier`, `DecisionTreeClassifier`, `LogisticRegression`, and `SVC`;
- Hyperparameter tuning via `RandomizedSearchCV`;
- **Best model**: `SVC` with RBF kernel
  **ROC-AUC = 0.90** on test data.

### Customer Segmentation

A key group identified: **High Risk + High Profit**

**Segment Characteristics:**
- High profitability (average revenue = 5,295 RUB);
- Average session time = 10 minutes;
- Nearly 50% of customers do **not** participate in promotions.

**Recommendations:**
- Personalized promo offers;
- Use of recommendation systems and gamification;
- Improve site navigation to enhance engagement.

---

## Conclusions

- The selected model demonstrates **high predictive accuracy** in identifying customers at risk of reduced activity;
- Data-driven segmentation allows targeted retention strategies for **high-value customers**;
- Recommended actions may improve **customer interaction time** and **overall activity**, benefiting the business.

---

Created by [Christina Lebedeva](https://github.com/chris-lebedeva)
