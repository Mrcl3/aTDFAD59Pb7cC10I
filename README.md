# Project Overview

This project focuses on predicting customer happiness based on survey responses from a select customer cohort in the logistics and delivery domain. The main objective is to analyze the provided dataset, preprocess the data, and build classification models to predict customer happiness.

## Approach

1. **Exploratory Data Analysis and Preprocessing**

   - Perform dataset exploration to gain insights into the data.
   - Handle missing values, if any, by applying appropriate strategies such as imputation or removal.
   - Identify and handle outliers using the Isolation Forest algorithm, considering a 10% baseline for outlier detection.
   - Analyze feature correlations using correlation matrices to understand the relationships between variables.

2. **Classification Models (80-20 Split)**

   - Choose classification models based on the LazyPredict library, which provides a quick overview of model performance.
   - Select a random state for training and testing data splits to ensure reproducibility.
   - Train and evaluate classification models such as XGBoost, ExtraTreesClassifier, DecisionTreeClassifier, and RandomForestClassifier.
   - Optimize the parameters of XGBoost using cross-validation and grid search.
   - Conduct SHAP (SHapley Additive exPlanations) analysis on the XGBoost model to interpret feature importances.
   - Optimize the parameters of ExtraTreesClassifier using cross-validation and grid search.
   - Conduct SHAP analysis on the ExtraTreesClassifier model to interpret feature importances.

3. **Data Augmentation**

   - Apply data augmentation techniques, starting with the Synthetic Minority Over-sampling Technique (SMOTE), to address class imbalance if present.
   - Consider downsizing the data and adjusting skewness to improve the performance of the classification models.
   - Evaluate the performance of the augmented data using XGBoost and ExtraTreesClassifier models.

4. **Feature Engineering**

   - Identify less significant features based on analysis and domain knowledge.
   - Remove or transform these less significant features.
   - Evaluate the performance of the models after feature engineering to assess the impact on predictive accuracy.

The project aims to provide insights into customer happiness prediction, assess the performance of different classification models, apply data augmentation techniques, and optimize feature engineering to improve predictive accuracy. Throughout the process, it's important to document findings and observations, and communicate the results effectively.

