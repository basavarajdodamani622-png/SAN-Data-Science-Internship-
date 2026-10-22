# Level 3 Task 1: Feature Engineering and Model Comparison

## 1. Project Overview

This project predicts student Grade Point Average (GPA) using academic performance and student-support information. It demonstrates feature engineering, regression modelling, model evaluation, and model comparison.

## 2. Dataset

- **Dataset:** Student Performance Dataset
- **Rows:** 2,392
- **Original cleaned dataset columns:** 15
- **Target variable:** GPA
- **Data file:** `cleaned_student_performance.csv`

## 3. Tools and Libraries

- Python
- Jupyter Notebook
- pandas and NumPy
- Matplotlib
- scikit-learn

## 4. Feature Engineering

Three additional features were created:

- `StudyTimePerAbsence`: weekly study time divided by absences plus one
- `TotalSupport`: tutoring plus parental support
- `ExtracurricularCount`: sum of extracurricular activities, sports, music, and volunteering

The target variable is `GPA`. `GradeClass` and `StudentID` were excluded from the model inputs. Categorical input features were encoded using one-hot encoding.

## 5. Methodology

1. Loaded and inspected the cleaned dataset.
2. Created three engineered features.
3. Split the data into 80% training and 20% testing data.
4. Used `random_state=42` for a reproducible split.
5. Compared a mean-GPA baseline, Linear Regression, and Random Forest Regression.
6. Evaluated performance using MAE, RMSE, and R².
7. Created model-comparison and actual-versus-predicted visualisations.

## 6. Model Results

| Model             |    MAE |   RMSE |      R² |
| ----------------- | -----: | -----: | ------: |
| Baseline          | 0.7660 | 0.9097 | -0.0008 |
| Linear Regression | 0.1554 | 0.1968 |  0.9531 |
| Random Forest     | 0.1810 | 0.2322 |  0.9348 |

## 7. Conclusion

Linear Regression performed best among the tested models, with the lowest MAE and RMSE and the highest R². Its R² score of approximately 0.9531 indicates that it explained about 95.31% of the variation in GPA on this test set.

These results apply to this dataset and test split. They do not establish causal relationships, and additional testing would be needed before real-world use.

## 8. Project Files

- `Level_3_Task_1_Feature_Engineering_Model_Comparison.ipynb` — analysis and modelling code
- `cleaned_student_performance.csv` — input dataset
- `model_comparison_results_updated.csv` — latest model comparison results
- `model_comparison_results.csv` — earlier results file
- `charts/model_comparison_mae.png` — model error comparison chart
- `charts/actual_vs_predicted_gpa.png` — actual versus predicted GPA chart
