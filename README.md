# Fraud Detection in Insurance Claims

## Project Purpose

The primary objective of this project is to develop a machine learning model that can detect fraudulent insurance claims. Fraudulent claims can result in significant financial losses for insurance companies, making accurate detection crucial. This project aims to create an efficient and accurate fraud detection system using machine learning techniques.

## Project Workflow

1- Data Preprocessing:

* Load and clean the data.

* Handle missing values and duplicates.

* Remove unnecessary features.

* Encode categorical variables and scale numerical features.

2- Exploratory Data Analysis (EDA):

* Analyze the distribution of features.

* Visualize correlations and identify patterns.

3- Clustering Approach:

* Initially applied clustering algorithms (K-Means, Agglomerative Clustering, DBSCAN) to group similar claims.

* Evaluated clustering performance using silhouette scores and ARI.

Found that clustering did not align well with actual fraud labels.

Supervised Learning Approach:

Implemented classification models: Logistic Regression, Random Forest, XGBoost.

Evaluated models using accuracy, precision, recall, F1-score, confusion matrix, and ROC curve.

Performance Comparison:

Logistic Regression and XGBoost performed the best with 75% accuracy.

Models struggled with detecting the minority class (fraud), highlighting data imbalance issues.

Recommendations:

Use techniques like SMOTE or class weighting to handle data imbalance.

Experiment with cost-sensitive learning and ensemble methods to improve recall for fraud cases.

Installation

To run the project, ensure you have the following libraries installed:

pip install pandas numpy scikit-learn xgboost seaborn matplotlib imbalanced-learn

Usage

Clone the repository:

git clone https://github.com/yourusername/insurance-fraud-detection.git

Navigate to the project directory:

cd insurance-fraud-detection

Run the Python script:

python fraud_detection.py

Results

The models developed showed moderate success in detecting fraudulent claims.

Further optimization is needed to improve the recall of fraudulent cas
