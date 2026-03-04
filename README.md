📌 German Credit Risk Prediction using Logistic Regression

📖 Project Overview

This project applies Logistic Regression to classify customers as Good Credit Risk or Bad Credit Risk using the German Credit Dataset.

The goal is to build a reliable classification model that can assist financial institutions in evaluating loan applications and minimizing the risk of default.

🎯 Objective

The main objectives of this project are:

Perform complete data preprocessing

Implement Logistic Regression for binary classification

Evaluate model performance using standard metrics

Interpret results with practical financial insights

Analyze feature impact using coefficients and odds ratios

🗂 Dataset Information

Dataset: German Credit Dataset

Target Variable: Credit_Risk (Good / Bad)

Features: Financial and demographic details of customers

The dataset contains structured financial attributes used to assess creditworthiness.


⚙️ Implementation Workflow

The notebook follows a structured machine learning pipeline:

Import Libraries

Load Dataset

Data Preprocessing

Handling categorical features

Encoding categorical variables

Feature scaling

Train-Test Split

Model Implementation (Logistic Regression)

Model Evaluation

Confusion Matrix

ROC Curve & AUC

Interpretation of Results

Question & Answer Section

🧠 Algorithm Used
🔹 Logistic Regression

Logistic Regression is a supervised learning algorithm used for binary classification problems.

It uses the Sigmoid Function to convert linear outputs into probabilities between 0 and 1.

Classification Rule:

If probability > 0.5 → Good Credit

If probability ≤ 0.5 → Bad Credit

📊 Evaluation Metrics

The model performance is evaluated using:

✅ Accuracy

✅ Precision

✅ Recall

✅ F1-Score

✅ Confusion Matrix

✅ ROC Curve

✅ AUC Score

⭐ Important Metric: Recall for Bad Credit

Recall is especially important in credit risk prediction.

Failing to correctly identify risky customers (low recall for Bad Credit) may result in financial losses. Therefore, improving recall for Bad Credit cases is critical.

📈 ROC Curve & AUC

The ROC Curve illustrates the trade-off between:

True Positive Rate (Sensitivity)

False Positive Rate

The AUC (Area Under Curve) measures the model’s ability to distinguish between Good and Bad credit applicants.

AUC close to 1 → Strong classification performance

AUC close to 0.5 → Weak model performance

📌 Model Coefficients & Odds Ratio

Coefficients indicate the change in log-odds of the target variable.

Positive coefficient → Increases probability of Good Credit

Negative coefficient → Increases probability of Bad Credit

Odds Ratio Calculation
np.exp(model.coef_)
Interpretation:

Odds Ratio > 1 → Positive impact on Good Credit

Odds Ratio < 1 → Negative impact on Good Credit

Odds Ratio = 1 → No significant impact

🛠 Technologies Used

Python

Pandas

NumPy

Matplotlib

Scikit-learn

Google Colab

📌 Results Summary

The model achieved good overall accuracy.

ROC-AUC score indicates strong classification capability.

The model performs better in identifying Good Credit customers.

Improvement is required in detecting Bad Credit customers to reduce financial risk.

🚀 How to Run the Project

Open the notebook in Google Colab

Upload the German Credit Dataset

Run all cells sequentially

View evaluation metrics and visualization outputs



📌 Conclusion

This project demonstrates the real-world application of Logistic Regression in financial risk analysis.

By applying systematic preprocessing, model training, and evaluation, the system successfully predicts credit risk with interpretable and meaningful results.

The model provides valuable insights that can support data-driven decision-making in banking and financial institutions.
