# Credit Risk Modeling

This repository contains an end-to-end **Credit Risk Modeling** project focused on predicting the likelihood that a loan applicant will default. Using a dataset provided by *Codebasics.io* with historical loan and borrower information, the objective is to build a machine learning model to classify borrowers as *low* or *high* risk of default. The project covers the full workflow from initial data analysis and feature engineering to model training and evaluation, and finally deploys the best model in a simple web application for interactive credit risk prediction.

## Project Workflow

1. **Exploratory Data Analysis (EDA):** Performed an initial analysis of the data to understand feature distributions and detect data quality issues.

2. **Feature Engineering:** Created and transformed features (e.g., one-hot encoding, ratios) that improve model performance and interpretability.

3. **Handling Class Imbalance:** Applied resampling techniques like **SMOTE** and **under-sampling** to deal with imbalanced data (few default cases).

4. **Model Training:** Built and compared multiple models including **Logistic Regression**, **Random Forest**, and **XGBoost**. Tuned hyperparameters for optimal results.

5. **Model Evaluation:** Assessed models using accuracy, precision, recall, F1-score, and ROC AUC. The XGBoost model performed the best overall.

## Model Performance

| Model                 | Accuracy | Precision | Recall | F1 Score | ROC AUC |
|-----------------------|----------|-----------|--------|----------|---------|
| Logistic Regression   | 0.92     | 0.70      | 0.50   | 0.58     | 0.75    |
| Random Forest         | 0.94     | 0.72      | 0.60   | 0.65     | 0.82    |
| XGBoost               | 0.95     | 0.74      | 0.62   | 0.67     | 0.85    |

## Tech Stack

- **Python**
- **Pandas**, **NumPy**
- **Scikit-learn**
- **XGBoost**
- **Imbalanced-learn**
- **Joblib**
- **Streamlit**

## Streamlit Application

The trained model was deployed using **Streamlit**. Users can input loan and customer details to:
- Predict default probability
- Generate a credit score (scaled)
- Assign a risk rating (e.g., Poor, Average, Good, Excellent)

## Lessons Learned

This project taught me the importance of properly handling imbalanced data, evaluating models with recall and precision (not just accuracy), and deploying interpretable models. It reinforced my understanding of how ML is applied in real-world finance and helped me gain practical experience building end-to-end systems.
