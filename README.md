# AI-Based Disease Risk Prediction & Explainability System

**Author:** Balaji  
**Environment:** Google Colab  
**Dataset:** UCI Heart Disease (Cleveland subset; UCI dataset ID 45)  
**Stack:** Python, pandas, scikit-learn, XGBoost, SHAP

## Overview
An educational tabular machine-learning project that groups the UCI Heart Disease target into a binary dataset label, compares Logistic Regression, Random Forest and XGBoost, evaluates held-out performance, and demonstrates model explainability. It includes preprocessing, metrics, plots, permutation importance, a held-out-record prediction and model/report export.

## Repository structure
```
ai-based-disease-risk-prediction/
├── notebooks/AI_Based_Disease_Risk_Prediction_System.ipynb
├── reports/README.md
├── .gitignore
├── LICENSE
├── README.md
└── requirements.txt
```

## Dataset
The notebook retrieves UCI Heart Disease dataset ID 45 using `ucimlrepo`. Internet access is required in Colab. The original target values 0–4 are converted to a binary label (`0` remains 0; values greater than 0 become 1). This is a project-specific grouping and is not a clinical definition.

## Run in Google Colab
1. Open the notebook in Colab.
2. Select a Python runtime.
3. Run cells from top to bottom.
4. Review the dataset, class distribution and held-out test metrics.
5. Inspect model explanations and exported artifacts.

## Models and evaluation
Logistic Regression, Random Forest and XGBoost (if available) are compared using accuracy, precision, recall, F1-score and ROC-AUC. The selected model is chosen by held-out ROC-AUC, with F1 as a tie-breaker. The notebook also produces a confusion matrix, ROC curve and permutation importance. Metrics are generated at runtime and are not fabricated in this repository.

## Responsible use
**This is not a medical device, screening tool or diagnosis.** Dataset scores are not individual clinical risk estimates. The dataset is small and historical; external clinical validation, qualified medical oversight, privacy/security review and regulatory assessment would be required before any real-world clinical use. Never use predictions as the sole basis for medical or other consequential decisions.

## Author
Balaji
