# Credit Card Fraud Detection

This project focuses on detecting fraudulent credit card transactions using a variety of machine learning techniques. It includes end-to-end processing—from data cleaning and exploratory analysis to feature engineering, model training, and performance evaluation.

##  Objective

The goal is to build accurate and sensitive models that can effectively detect anomalies in credit card transactions, minimizing false positives and false negatives. This is crucial for maintaining financial security and reducing fraud losses.

##  Dataset

The dataset used in this project contains anonymized credit card transaction data, where:

- Features are numerical and scaled for privacy
- \`Class = 1\` indicates a fraudulent transaction
- \`Class = 0\` indicates a legitimate transaction

 [Credit Card Fraud Detection – Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)


##  Key Steps

### 1. Data Preprocessing
- Handling missing values and duplicates
- Exploratory Data Analysis (EDA) to understand distribution and correlation
- Outlier detection and removal
- Feature scaling using StandardScaler and MinMaxScaler

### 2. Feature Engineering
- Sequential Forward Selection (SFS)
- Backward Stepwise Selection (BSS)
- Feature correlation adjustments to optimize model input

### 3. Model Training & Evaluation
Several classification algorithms were evaluated:

| Model                    | Accuracy | Sensitivity |
|-------------------------|----------|-------------|
| Logistic Regression      | 0.730    | 0.675       |
| Linear Discriminant Analysis (LDA) | 0.727 | 0.667 |
| Decision Tree            | 0.737    | 0.682       |
| Gradient Boosting        | 0.736    | 0.695       |
| K-Nearest Neighbors (KNN)| 0.737    | 0.677       |
| QDA                      | 0.720    | 0.589       |
| Random Forest            | 0.735    | 0.694       |
| Support Vector Classifier| 0.734    | 0.660       |

Metrics like confusion matrix, classification report, and objective value (weighted accuracy + sensitivity) were used for evaluation.

##  Best Performing Models

- **Gradient Boosting** achieved the best balance between accuracy and sensitivity.
- **Random Forest** and **Decision Tree (tuned)** also performed robustly.

##  Requirements

Install dependencies with:

\`\`\`bash
pip install -r requirements.txt
\`\`\`

Or install key libraries manually:

\`\`\`bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
\`\`\`


##  Future Work

- Incorporate real-time detection with streaming data
- Use deep learning models like Autoencoders or LSTMs
- Apply anomaly detection techniques (e.g., Isolation Forest)



