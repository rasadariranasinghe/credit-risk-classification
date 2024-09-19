# Credit Risk Analysis

## Project Overview

This project aims to analyze credit risk by building a logistic regression model to classify loans as either healthy or high-risk. Using historical loan data, the model is trained to predict the likelihood of default, helping financial institutions make more informed lending decisions.

## Technologies Used

- **Python** (version 3.x)
- **Pandas** (for data manipulation)
- **scikit-learn** (for logistic regression and performance evaluation)
- **NumPy** (for numerical operations)
- **Jupyter Notebook** (for interactive coding)
- **Git/GitHub** (for version control and collaboration)

## Data Source

The dataset used in this analysis, `lending_data.csv`, contains historical loan records with features such as loan amount, income, and credit score, along with the `loan_status` column that serves as the target variable.

- **0**: Healthy loan (low risk of default)
- **1**: High-risk loan (high risk of default)

## Modeling Process

1. **Data Preparation**:
   - The data is read from `lending_data.csv`.
   - The target variable (`y`) is the `loan_status` column.
   - The feature set (`X`) consists of all other columns.

2. **Training and Testing Split**:
   - The dataset is split into training and testing sets using `train_test_split` with a random state of 1 to ensure reproducibility.

3. **Model Training**:
   - A logistic regression model is trained using the training data.

4. **Model Evaluation**:
   - Predictions are made on the test data.
   - Performance is evaluated using a confusion matrix and classification report.

## Results

- **Accuracy**: 99%
- **Precision**:
  - Healthy Loans (0): 100%
  - High-Risk Loans (1): 85%
- **Recall**:
  - Healthy Loans (0): 99%
  - High-Risk Loans (1): 91%

### Key Insights:

- The model is highly effective in predicting healthy loans with perfect precision and near-perfect recall.
- For high-risk loans, the recall is strong (91%), meaning most high-risk loans are correctly identified. Precision for high-risk loans is 85%, indicating some healthy loans are misclassified as high-risk.
