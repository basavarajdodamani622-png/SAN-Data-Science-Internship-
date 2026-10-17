# Reproducible Data Science Project

## Project Overview

This project analyzes student performance and predicts GPA using machine learning.

## Dataset

- Source: Existing cleaned Student Performance dataset from Level 1, Task 1.
- File: cleaned_student_performance.csv
- Rows: 2392
- Columns: 15

## Tools

- Python
- pandas and NumPy
- Matplotlib
- scikit-learn
- Jupyter Notebook

## Workflow

1. Load and validate the cleaned dataset.
2. Perform exploratory data analysis (EDA).
3. Visualize GPA, study time, tutoring, and absences.
4. Train a Linear Regression model to predict GPA.
5. Evaluate predictions using MAE, RMSE, and R-squared.
6. Save model results and charts.

## Model Evaluation

- Model: Linear Regression
- MAE: 0.1553
- RMSE: 0.1966
- R-squared: 0.9532

## Key Finding

The model explains approximately 95.32% of the variation in GPA on the test set. This result applies to this dataset and test split.

## Learning

This project demonstrates data validation, EDA, visualization, model training, evaluation, and project documentation.

## How to Run the Project

1. Install Python on your computer.
2. Open the project folder in VS Code or Command Prompt.
3. Install the required libraries using:

   pip install -r requirements.txt

4. Open the Jupyter Notebook.
5. Run all notebook cells from top to bottom.

## Project Files

- `Level_3_Task_3_Reproducible_Data_Science_Project.ipynb` — project analysis and model.
- `cleaned_student_performance.csv` — dataset used in this project.
- `model_evaluation_results.csv` — model evaluation metrics.
- `charts/` — saved project visualizations.
- `requirements.txt` — required Python libraries.
