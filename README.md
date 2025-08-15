# BigMartAnalysis

## Observations and approach

1. Performed basic EDA like checking missing values and duplicates
2. Identified all categorical columns and did basic plotting
3. Checked the unique values of categorical columns and confirmed that test set does not contain 
completely new values that are not in train set.
4. Missing values in Item Weight column is filled with uinique item weight of Item identifier
5. Missing values in Outlet Size is filled with the help of Outlet type & Outlet_Location_Type
6. Created baseline model using RandomForest Regressor with default parameters and got RMSE close 1200
7. Created different models like Catboost, Xgboost along with hyperparameter tuning using Optuna library
8. CatboostRegressor + Optuna combination gave best result with RMSE = 1149 so far.
