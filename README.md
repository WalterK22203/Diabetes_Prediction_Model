# Diabetes Prediction Model

This project builds a machine learning workflow to predict diabetes outcomes from clinical measurements. The notebook loads a diabetes dataset, inspects data quality, visualizes relationships between variables, trains classification models, and compares model performance.

## Dataset

- Source: [Kaggle Diabetes dataset by Ehab Aboelnaga](https://www.kaggle.com/datasets/ehababoelnaga/diabetes-dataset)
- License: Apache 2.0
- Local file: `Healthcare-Diabetes.csv`

The dataset includes patient-level health measurements such as pregnancies, glucose, blood pressure, skin thickness, insulin, BMI, diabetes pedigree function, age, and the target variable `Outcome`.

## Tools And Technologies

- Python
- Jupyter Notebook
- pandas and NumPy
- matplotlib and seaborn
- scikit-learn
- Git and GitHub

## Project Structure

```text
Diabetes_Prediction_Model/
    Final_Project.ipynb
    Healthcare-Diabetes.csv
    requirements.txt
    README.md
    .gitignore
```

## Setup

Create and activate a virtual environment:

```powershell
python -m venv .venv
.venv\Scripts\activate
python -m pip install --upgrade pip
```

Install dependencies:

```powershell
pip install -r requirements.txt
```

Open `Final_Project.ipynb` in VS Code or Jupyter and run all cells.

## Machine Learning Workflow

1. Import the required Python libraries.
2. Load `Healthcare-Diabetes.csv`.
3. Inspect dataset shape, missing values, duplicate rows, and class distribution.
4. Review descriptive statistics.
5. Visualize feature correlations with a heatmap.
6. Split features and target values.
7. Clean clinically impossible zero values in selected medical measurements.
8. Remove the row identifier from model features.
9. Use reproducible scikit-learn preprocessing pipelines.
10. Train and evaluate Random Forest and Logistic Regression classifiers.
11. Compare accuracy, precision, recall, F1 score, and ROC-AUC.
12. Tune the Random Forest model and interpret feature importance.

## Key Improvements

- Removed `Id` from model training because it is a row identifier.
- Treated clinically impossible zero measurements as missing values.
- Moved imputation and scaling into scikit-learn pipelines.
- Added stratified cross-validation for more stable model evaluation.
- Added ROC-AUC, ROC curves, precision-recall curves, and confusion matrix heatmaps.
- Tuned the Random Forest model with `GridSearchCV`.
- Added permutation feature importance for model interpretation.

## Expected Outputs

The notebook should display:

- Dataset shape and schema
- Missing value and duplicate checks
- Class distribution
- Descriptive statistics
- Correlation heatmap
- Cross-validation results
- Random Forest, tuned Random Forest, and Logistic Regression metrics
- Confusion matrix, ROC curve, and precision-recall curve
- Permutation feature importance
- Model comparison table and chart

## Model Limitations

This project is an educational machine learning workflow. It is not a medical diagnosis tool and should not be used to make clinical decisions. The dataset is limited in size and scope, and model performance should be validated on additional representative data before any real-world use.

## Security And Privacy

Do not commit Kaggle API tokens, passwords, API keys, private patient data, or local virtual environments. The `.gitignore` file excludes common local and sensitive files.

## Dataset Credit

Dataset credit belongs to Ehab Aboelnaga on Kaggle. The dataset is published under the Apache 2.0 license according to the Kaggle dataset page.
