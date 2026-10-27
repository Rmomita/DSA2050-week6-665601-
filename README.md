




## Student Information
- Student Name: Racheal Momita
- Student ID: 665601

## Lab Objective
The objective of this lab was to build and evaluate regression models for predicting sales using advertising spend, store visits, discounts, region, customer segment, and product category. The models were compared against baseline predictions to identify the most accurate approach.

## Models Compared
- Mean Baseline
- Median Baseline
- Linear Regression
- Ridge Regression
- Decision Tree Regression

## Best Model
Ridge Regression with alpha = 10 achieved the lowest test MAE in the alpha-tuning experiment.

Selected Model MAE: KES 13,624.90

## Two Key Findings
1. Ridge Regression substantially outperformed both baseline models, demonstrating that using the available features provides more accurate sales predictions than predicting a constant mean or median.
2. Prediction errors varied across customer segments. Retail had the highest MAE (KES 15,560.58), while SME had the lowest MAE (KES 10,481.46).

## Three Limitations
1. The dataset contains only 320 observations, which may limit generalisation to new sales data.
2. Important factors such as seasonality, competitor prices, stock availability, and changing customer behaviour are not included.
3. Predictive relationships do not establish causation; the model cannot prove that advertising spending or discounts directly cause changes in sales.

## Final Recommendation
Ridge Regression is a promising candidate for sales prediction. Before deployment, the selected hyperparameter should be validated using cross-validation on the training data, followed by final evaluation on an untouched test set. Performance should also be monitored across customer segments and over time.

