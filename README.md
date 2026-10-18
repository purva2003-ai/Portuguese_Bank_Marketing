# Portuguese Bank Marketing

## Project Overview

This project analyzes data from Portuguese bank marketing campaigns and develops machine learning models to predict whether a customer will subscribe to a term deposit.

The project focuses on data analysis, customer behavior, predictive modeling, and business recommendations for improving future marketing campaigns.

---

## Project Objectives

The main objectives of this project are:

1. Perform complete data analysis on the Portuguese Bank Marketing dataset.
2. Understand customer characteristics and campaign-related factors.
3. Build machine learning models to predict term deposit subscription.
4. Compare multiple classification models.
5. Identify important features used by the models.
6. Provide recommendations to the bank marketing team.

---

## Dataset

The dataset contains information from direct marketing campaigns of a Portuguese banking institution.

The target variable is:

- `y` — whether the customer subscribed to a term deposit (`yes` / `no`).

The `duration` feature was excluded from the predictive model because it is only known after the call and would not be available when deciding which customers to contact.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Joblib
- VS Code

---

## Project Workflow

```text
Data Collection
       ↓
Data Cleaning
       ↓
Exploratory Data Analysis
       ↓
Feature Preparation
       ↓
Train/Test Split
       ↓
Data Preprocessing
       ↓
Machine Learning
       ↓
Model Comparison
       ↓
Feature Importance
       ↓
Business Recommendations

---

## Project Limitations

1. **Imbalanced target variable:** Most customers did not subscribe to a term deposit. Accuracy alone may therefore be misleading, so precision, recall, and F1-score should also be considered.

2. **Model performance:** The models may miss potential subscribers. Predictions should be evaluated alongside business costs and campaign objectives.

3. **Feature interpretation:** Feature importance indicates which variables the Random Forest uses most in its predictions. It does not establish that these variables cause subscription.

4. **Exclusion of duration:** The `duration` feature was excluded because call duration is only known after the call. Including it would cause data leakage for a model intended to select customers before contacting them.

5. **Historical data:** The dataset represents historical marketing campaigns. Customer behavior and economic conditions may change, so model performance should be monitored on newer data.

6. **Business validation:** The model should support marketing decisions rather than replace human judgment. Recommendations should be tested before being applied widely.

---

## Installation and Usage

### Prerequisites

- Python installed on your computer
- Visual Studio Code
- The Jupyter extension in VS Code

### 1. Open the Project

Open the `Portuguese_Bank_Marketing` project folder in VS Code.

### 2. Install Required Libraries

Open the VS Code terminal using **Terminal → New Terminal** and run:

```bash
python -m pip install -r requirements.txt
```

### 3. Open the Jupyter Notebook

Open:

`notebooks/Portuguese_Bank_Marketing.ipynb`

Select a Python kernel that has the required libraries installed.

### 4. Run the Notebook

Run the notebook cells from top to bottom in order. If prompted, install missing dependencies in the selected Python environment.

### 5. Check the Outputs

The project stores its generated files in the following folders:

- `data/` — original and cleaned datasets
- `outputs/` — model comparison results, feature importance, job analysis, and charts
- `models/` — saved machine-learning models and the complete prediction pipeline

**Note:** Run the notebook from its expected project structure so that relative file paths work correctly.