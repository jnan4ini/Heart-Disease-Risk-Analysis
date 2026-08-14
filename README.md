# Heart-Disease-Risk-Analysis
Heart disease risk analysis and predictive modeling using Python, logistic regression, and decision trees.
# Heart Disease Risk Prediction & Analysis

## Project Overview

This project explores whether non-invasive clinical measurements can be used to predict heart disease risk using data analysis and machine learning.

Using the Cleveland heart disease dataset, I cleaned and analyzed patient data, explored relationships between clinical variables, and developed predictive models to identify patients at higher risk of heart disease.

The project demonstrates an end-to-end analytical workflow including data cleaning, exploratory data analysis, visualization, predictive modeling, model evaluation, and interpretation of results.

## Research Question

Can machine learning be used to predict heart disease using simple, non-invasive clinical measurements?

## Dataset

The project uses the Cleveland heart disease dataset sourced from the UCI Machine Learning Repository via Kaggle.

After removing duplicate observations, the final dataset contained:

- 302 patient observations
- 14 variables

Variables included patient characteristics and clinical measurements such as:

- Age
- Sex
- Chest pain type
- Resting blood pressure
- Cholesterol
- Maximum heart rate
- ST depression
- Heart disease outcome

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn
- Jupyter Notebook

## Data Analysis Process

### 1. Data Cleaning

The dataset was imported using Pandas and checked for duplicate observations. Duplicate records were removed before analysis to reduce the risk of biased model results.

### 2. Exploratory Data Analysis

Descriptive statistics and visualizations were used to examine distributions and relationships between patient characteristics and heart disease outcomes.

The analysis focused particularly on clinical indicators including maximum heart rate and ST depression.

### 3. Feature Selection

Selected predictors included:

- Age
- Sex
- Chest pain type
- Resting blood pressure
- Cholesterol
- Maximum heart rate
- ST depression

### 4. Predictive Modeling

Two supervised machine-learning models were developed:

**Logistic Regression**

A classification model used to estimate the probability of heart disease based on selected clinical characteristics.

**Decision Tree**

A Decision Tree Classifier was used to identify decision rules and relationships between patient characteristics and predicted heart disease outcomes.

The Decision Tree was limited to a maximum depth of 3 to reduce overfitting.

### 5. Model Evaluation

The data was divided into training and testing sets using an 80/20 split.

Model performance:

| Model | Test Accuracy |
|---|---:|
| Logistic Regression | 90.16% |
| Decision Tree | 81.97% |

Logistic Regression produced the highest test-set accuracy.

To evaluate model stability beyond a single train-test split, I also performed 10-fold cross-validation on the Logistic Regression model.

**10-Fold Cross-Validation Results**

- Mean Accuracy: 80.84%
- Accuracy Standard Deviation: 0.0717

The cross-validation results provide a more realistic estimate of how the model may perform across different samples.

## Key Findings

The analysis showed that non-invasive clinical measurements contain useful information for predicting heart disease risk.

The Decision Tree analysis highlighted variables including ST depression and chest pain type as important components of the classification process.

While the initial Logistic Regression test accuracy reached 90.16%, 10-fold cross-validation produced a mean accuracy of 80.84%, demonstrating the importance of evaluating predictive models across multiple data samples rather than relying on a single train-test split.

## Limitations

The dataset contains only 302 observations after cleaning, which limits the generalizability of the results.

Cross-validation also showed variation in model performance across different subsets of the data.

Future analysis could evaluate additional models and larger datasets to improve predictive performance and model stability.

## Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis
- Data Visualization
- Statistical Analysis
- Logistic Regression
- Decision Trees
- Machine Learning
- Model Evaluation
- Cross-Validation
- Python
- Pandas
- scikit-learn
- Analytical Communication

## Project Files

- `Heart_Disease_Risk_Analysis.pdf` — Full project report including code, visualizations, model results, and interpretation
- `heart_disease_analysis.ipynb` — Jupyter Notebook containing the analysis and Python code (if available)
- `heart.csv` — Dataset used for analysis (if included)

## Author

**Nandini Jaggavarapu**

M.S. Quantitative Economics  
University of Connecticut
