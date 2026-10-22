# Level 3 - Task 2: Time Series Forecasting

## Project Overview
This project analyzes monthly sales for a global e-commerce dataset
and compares two forecasting methods.

## Dataset
- Source: Global E-Commerce Sales & Customer Analytics
- File: global_ecommerce_sales (2).csv
- Records: 2,000
- Columns: 15
- Date range: January 2023 to December 2025
- Target: Total_Sales

## Methodology
1. Converted Order_Date to datetime format.
2. Aggregated daily transactions into monthly sales.
3. Visualized the monthly sales trend.
4. Used January 2023 to December 2024 for training.
5. Used January 2025 to December 2025 for testing.
6. Compared a training-average baseline with Linear Regression.

## Results

| Model | MAE | RMSE |
|---|---:|---:|
| Baseline (Training Average) | 2852.81 | 3361.29 |
| Linear Regression | 2806.74 | 3341.72 |

## Conclusion
Linear Regression performed slightly better than the baseline
on both MAE and RMSE. However, the improvement was small.
Monthly sales fluctuated, so additional seasonal forecasting
methods may improve future predictions.

## Output Files
- monthly_sales_trend.png
- actual_vs_forecasted_sales.png
- sales_forecast_results.csv
- Level_3_Task_2_Time_Series_Forecasting.ipynb
- README.md
