# Customer Activity Analysis and Forecasting for "One Click" Online Store

This project focuses on predicting customer activity decline for the **"One Click"** online store and identifying customer segments that require retention actions.

## Project Goal

Build a machine learning model to predict whether a regular customer's activity is likely to decrease in the next 3 months, and use the results to provide data-driven retention recommendations.

## Data

The project uses several datasets containing:

- customer behaviour and purchase preferences;
- marketing interaction data;
- revenue by period;
- website activity time;
- customer profit for the last three months.

## Workflow

The project includes:

- data overview and preprocessing;
- exploratory data analysis;
- merging several data sources into one modeling dataset;
- correlation analysis;
- model training and hyperparameter tuning;
- model interpretation using SHAP;
- customer segmentation based on predicted risk and profitability;
- business recommendations for customer retention.

## Models

The following classification models were trained and compared:

- `KNeighborsClassifier`
- `DecisionTreeClassifier`
- `LogisticRegression`
- `SVC`

Hyperparameter tuning was performed using `RandomizedSearchCV`.

## Results

The best-performing model was **SVC with RBF kernel**, achieving:

**ROC-AUC = 0.90** on the test set.

The model was used to identify customers with a high probability of decreased activity.

## Customer Segmentation

A key segment was identified:

**High Risk + High Profit**

This segment includes profitable customers who are likely to reduce their activity.

## Recommendations

To retain high-value customers at risk, the following actions were recommended:

- personalized promotional offers;
- recommendation systems;
- gamification mechanics;
- improved website navigation and user experience.

## Conclusion

The project demonstrates how machine learning can help an online store detect customers at risk of reduced activity and prioritize retention efforts for the most valuable customer segments.

---

Created by [Christina Lebedeva](https://github.com/chris-lebedeva)
