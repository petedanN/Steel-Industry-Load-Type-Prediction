# Steel Industry Load Type Prediction

## Overview
This project uses machine learning to predict the **Load_Type** in a steel manufacturing setting. The dataset includes energy usage, reactive power, and CO2 emissions, helping to classify operational load types for better efficiency.

## Dataset
- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/851/steel+industry+energy+consumption)
- **Origin**: Data was collected from DAEWOO Steel Co. Ltd in Gwangyang, South Korea. The company produces various types of steel coils, plates, and iron plates.
- **Size**: 35,040 records with 11 columns.
- **Features**: Includes energy consumption, power factors, CO2 emissions, and time-related data.
- **Target**: 'Load_Type' (categorical variable, e.g., 'Light_Load').

## Methodology
**1. Exploratory Data Analysis (EDA)**

  - Performed in-depth data exploration to understand feature distributions, correlations, and trends.

**2. Data Preprocessing**

 - Handled missing values and duplicates(if any).

 - Encoded categorical variables.

 - Standardized/normalized numerical features for consistency.

**3. Feature Selection**

 - Used SelectKBest to choose the most relevant features for the target variable.

**4. Model Training**

  Implemented and compared the following models:

 - Logistic Regression

 - Decision Tree
  
 - Support Vector Machine (SVM)

 - Multi-Layer Perceptron (MLP)

 - XGBoost (Best Model)

**5. Hyperparameter Tuning**

 - Performed grid search  for XGBoost.

**6. Results**

 - Accuracy: 91%

**7. Deployment**

 - The trained XGBoost model and preprocessing steps were saved as a pipeline in "**xgboost_pipeline.pkl.**"
