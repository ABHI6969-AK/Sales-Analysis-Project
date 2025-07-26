Here's a shorter and more precise README file for your GitHub project:

# D-Mart Sales Prediction

## Project Goal

This project aims to build a predictive model for `Item_Outlet_Sales` using historical D-Mart sales data. The model helps identify product and outlet properties that drive sales growth.

## Dataset

The dataset contains 2013 sales data for 1559 products across 10 D-Mart stores in various cities, including product and store attributes. Missing values are present and handled.

## Key Steps

1.  **Data Preprocessing**: Handles missing `Item_Weight` (mean imputation) and `Outlet_Size` (mode imputation). Standardizes `Item_Fat_Content` categories.
2.  **Feature Engineering**: Creates `Item_Type_Combined` and `Years_Operating`.
3.  **Exploratory Data Analysis (EDA)**: Visualizes sales distribution, correlations, and sales by `Outlet_Type`.
4.  **Feature Encoding**: Applies Label Encoding to `Outlet_Identifier` and One-Hot Encoding to other categorical features.
5.  **Model Training**: Uses a `RandomForestRegressor` with 200 estimators. Evaluates performance using 5-fold cross-validation (RMSE).
6.  **Prediction**: Generates sales predictions for the test dataset.

## Technologies Used

* Python
* pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn

## How to Run

1.  Clone the repository.
2.  Ensure `train.csv` and `test.csv` are accessible (update paths if necessary).
3.  Install dependencies: `pip install pandas numpy matplotlib seaborn scikit-learn`
4.  Run the script: `python ds_feb_batch_(minor_project)k_abhinav_d_martsales.py`

The script will output performance metrics, feature importances, and a `BigMart_Predictions.csv` file with the predicted sales.
