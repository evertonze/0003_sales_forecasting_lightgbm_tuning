## Overview
End-to-end time series forecasting project using LightGBM to predict sales.  
Focus on feature engineering, time-aware validation, and hyperparameter optimization.

## Dataset
- Historical sales data  
- Multiple categorical and temporal features  
- Target: sales volume  

## Methodology
1. Data cleaning and preprocessing  
2. Time-based feature engineering  
   - Year, month, day, week  
   - Lag features  
   - Rolling statistics  
3. Train/validation split using time-based strategy (no data leakage)  
4. Baseline LightGBM model  
5. Hyperparameter tuning  
6. Final model training on full dataset  

## Model
- LightGBM (Gradient Boosting)
- Optimized hyperparameters:
  - `num_leaves`
  - `max_depth`
  - `learning_rate`
  - `min_child_samples`
  - `feature_fraction`
  - `subsample`

## Evaluation
- Time-aware validation
- RMSLE as primary metric

## Results
- Performance improvement after hyperparameter tuning
- Reduced validation error compared to baseline

## Tech Stack
- Python
- pandas
- numpy
- LightGBM
- scikit-learn
- matplotlib / seaborn

## Key Concepts Applied
- Time series feature engineering  
- Gradient boosting  
- Model optimization  
- Leakage prevention  
- Forecasting workflow
