# MLOPs-A2-MSDSF23M014-MSDSF23M021
# Solution Discussion & Steps Performed
## 1. Data Loading and Cleaning:
- Extracted Data from Excel sheets for "ICT Morning" and "ICT Afternoon" ,"cloud computing morning" and "cloud computing afternoon" using pandas.
- Filled Missing values with zeros because we consider that students didn't attempted those activities.
- kept only only relevant columns (from the fourth column onwards) are retained
## 2. Normalization of Scores:
- Mapped the weightage/scale to all marks to convert them to their absolute value.
## 3. Data Exportation:
- Saved the normalized data for both morning and afternoon sessions as CSV files for further analysis.
## 4. Predictive Modeling:
- Used different machine learning models (XGBoost, RandomForest, Ridge, and LinearRegression) and trained them using the morning session data to predict the total scores from partial scores (first 5 activities, first 6 activities & so on).
- Used GridSearchCV  to tune the hyperparameters of each model based on cross-validation.
- Hence Predictions are made for the afternoon session data, and the absolute errors (average, maximum, and minimum) are calculated and saved.
## 5. Reporting:
- Saved all the Results into CSV files, showing both the actual and predicted totals for each student after incorporating scores from different assessments incrementally.
Also created another report to detail the average, maximum, and minimum absolute errors in predictions across different model configurations and subsets of assessment scores.
