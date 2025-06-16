# Credit-card-fraud-using-DL-with-AGSS

This project implements a machine learning pipeline to detect fraudulent transactions in credit card data. It addresses class imbalance using various oversampling techniques and evaluates model performance with multiple metrics.

📂 Dataset
Source: Kaggle Credit Card Fraud Detection Dataset

Description: Contains transactions made by European cardholders in September 2013, with anonymized features (V1 to V28), Amount, Time, and a binary Class (1 for fraud, 0 for normal).

📌 Features
Preprocessing:

Handles missing values.

Standardizes features using StandardScaler.

Imbalanced Learning:

Applies various oversampling techniques:

RandomOverSampler

SMOTE

ADASYN

BorderlineSMOTE

SVMSMOTE

KMeansSMOTE

Modeling:

Uses a basic feedforward neural network implemented in PyTorch.

Evaluation:

Computes Accuracy, Precision, Recall, and F1-Score.

🧠 Technologies Used
Python

PyTorch

Pandas, NumPy, Scikit-learn

imbalanced-learn (imblearn)

🚀 How to Run
Clone the repository or download the notebook.

Ensure you have the necessary libraries:

bash
Copy
Edit
pip install pandas numpy scikit-learn imbalanced-learn torch
Place the creditcard.csv dataset in the appropriate path (modify if needed in the notebook).

Run all cells in the notebook.

📊 Results
The notebook compares the effectiveness of different oversampling techniques in detecting fraudulent transactions by evaluating the classification performance metrics.

🧪 Oversampling Techniques Compared
Method	Accuracy	Precision	Recall	F1-Score
RandomOverSampler	✅	✅	✅	✅
SMOTE	✅	✅	✅	✅
ADASYN	✅	✅	✅	✅
BorderlineSMOTE	✅	✅	✅	✅
SVMSMOTE	✅	✅	✅	✅
KMeansSMOTE	✅	✅	✅	✅

✅ indicates that the model was trained and evaluated using that technique.

📎 Notes
Be sure to run in a GPU-supported environment for faster training.

Dataset is highly imbalanced; direct training without oversampling leads to poor fraud detection.
