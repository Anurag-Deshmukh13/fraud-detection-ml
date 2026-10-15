# Credit Card Fraud Detection Using Machine Learning

## Overview
This project uses machine learning to identify potentially fraudulent credit card transactions. It compares classification models and evaluates a tuned Random Forest model.

## Project Objectives
- Prepare and analyze transaction data.
- Train and compare machine learning models.
- Tune the Random Forest classifier.
- Evaluate performance using precision, recall, F1-score, ROC-AUC, and average precision.
- Select a classification threshold using out-of-fold training predictions.

## Final Model
**Model:** Tuned Random Forest

**Decision threshold:** 0.4048

## Test Results
- ROC-AUC: 0.9337
- Average precision: 0.8091
- Fraud precision: 97.22%
- Fraud recall: 73.68%
- Fraud F1-score: 0.8383

The test set contained 95 fraudulent transactions. The model detected 70 and missed 25, with 2 legitimate transactions incorrectly flagged.

## Repository Contents
- `fraud_detection.ipynb` — model training, evaluation, and visualizations.
- `fraud_model.joblib` — saved model package and decision threshold, if included.
- `requirements.txt` — Python dependencies.

## Limitations
The model does not detect every fraudulent transaction. The dataset is highly imbalanced, and the results may not generalize to different transaction populations. Feature importance scores do not establish causation.

## How to Run
1. Install the required packages using `pip install -r requirements.txt`.
2. Open the notebook in Jupyter or Google Colab.
3. Provide the appropriate dataset and run the notebook cells in order.

## Disclaimer
This is an educational machine learning project and should not be used as the sole basis for real financial fraud decisions without further validation.
