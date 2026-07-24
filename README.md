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
    REPLICATE_PROJECT_INSTRUCTIONS.txt
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
7. Train and evaluate a Random Forest classifier.
8. Review Random Forest feature importance.
9. Create a cleaned feature set by dropping selected columns.
10. Train a Random Forest model on the cleaned data.
11. Train a Logistic Regression model on scaled cleaned data.
12. Compare model accuracy, precision, recall, and F1 score.

## Expected Outputs

The notebook should display:

- Dataset shape and schema
- Missing value and duplicate checks
- Class distribution
- Descriptive statistics
- Correlation heatmap
- Random Forest metrics and feature importance
- Cleaned Random Forest metrics
- Logistic Regression metrics
- Model comparison table and chart

## Security And Privacy

Do not commit Kaggle API tokens, passwords, API keys, private patient data, or local virtual environments. The `.gitignore` file excludes common local and sensitive files.

## Dataset Credit

Dataset credit belongs to Ehab Aboelnaga on Kaggle. The dataset is published under the Apache 2.0 license according to the Kaggle dataset page.
