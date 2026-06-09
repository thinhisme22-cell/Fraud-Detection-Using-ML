# Fraud-Detection-Using-ML
## Overview
According to Nasdaq Verafin’s 2026 Global Financial Crime Report, global fraud causes nearly $580 billion in losses every year. This is a serious and growing problem, driven by more advanced criminal networks, security weaknesses, and the increasing misuse of AI. At the same time, AI can also be used as a powerful tool to fight back. If criminals can use AI to commit fraud, then financial institutions and analysts can use machine learning to monitor transactions, detect suspicious patterns, and reduce fraud more effectively. This project is built around that idea. The goal is to analyze financial transaction data, understand common fraud patterns, and train multiple classification models to compare their performance in detecting fraudulent transactions.
## Data Source
The dataset used in this project was retrieved from Kaggle, an open-source platform for datasets and machine learning projects. It contains 1,048,575 rows and 11 attributes related to financial transactions.
The dataset includes information such as transaction type, transaction amount, account balances before and after each transaction, and whether the transaction was identified as fraudulent.
The columns in the dataset include:
* step
* type
* amount
* nameOrig
* oldbalanceOrg
* newbalanceOrig
* nameDest
* oldbalanceDest
* newbalanceDest
* isFraud
* isFlaggedFraud

Dataset link: [Fraud](https://www.kaggle.com/datasets/tushar9999/fraud-detection/data)
## Algorithm
1. Decision Tree
2. Logistic Regression
3. XGBoost (eXtreme Gradient Boosting)
4. LightGBM (Light Gradient Boosting Machine)
## Quick Set Up
1. Clone the repository:
   ```bash
   git clone https://github.com/thinhisme22-cell/Fraud-Detection-Using-ML.git
   ```
2. Move into the project folder:
   ```bash
   cd Fraud-Detection-Using-ML
   ```
3. Install the required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost lightgbm jupyter
   ```
4. Download the dataset from the link above and place it in the project folder as:
   ```text
   Fraud.csv
   ```
5. Open the Jupyter Notebook:
   ```bash
   jupyter notebook fraud_detection.ipynb
   ```
## Conclusion
After training and evaluating the four models, Decision Tree and XGBoost showed the best overall performance. The Decision Tree model gave a good balance between precision and recall. It was able to detect many fraud cases while keeping false alarms relatively low. XGBoost achieved higher recall, meaning it was better at catching fraud cases. However, it also produced more false alarms compared to the Decision Tree model.
