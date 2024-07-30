# Fraud Detection in Online Payments
# An Analysis Using Machine Learning Techniques

## Abstract
In today's digital era, securing online payment transactions is paramount. This study leverages the "Online Payments Fraud Detection Dataset" from Kaggle, containing over 6 million transactions, to evaluate the efficacy of machine learning algorithms - Logistic Regression, Random Forest, Decision Trees, and Bagging Classifier - in detecting fraud. Preliminary results highlight Random Forest's proficiency in identifying complex transaction patterns. Emphasis is also placed on the role of features such as transaction type and amount in model accuracy. The research aims to enhance online transaction security and equip financial institutions with tools to mitigate fraud risks.

Keywords—Machine Learning, Algorithms, Logistic Regression, Random Forest, Decision Trees, Bagging

## Introduction
- Research Questions
How can machine learning algorithms be utilized to detect and classify fraudulent transactions in online payments?
How does the performance of different machine learning algorithms compare in terms of fraud detection accuracy and efficiency?
- Hypotheses
Hypothesis 1: Machine learning algorithms, such as logistic regression, decision trees, and random forests, can effectively classify fraudulent and non-fraudulent transactions in online payments.
Hypothesis 2: The inclusion of additional features, such as transaction amount, balance changes, and recipient details, will improve the accuracy and reliability of fraud detection models.

## Literature Review
This section reviews existing studies on fraud detection in online payments, emphasizing the effectiveness of various machine learning techniques.

## Methodology
### Data Source
The dataset for this study is the "Online Payments Fraud Detection Dataset" from Kaggle, consisting of 6,353,307 entries, each representing a distinct online payment transaction. The dataset includes 11 features, such as transaction type, amount, sender and receiver details, and fraud indicators.

### Descriptive Statistics
The dataset reveals patterns in transaction types, amounts, and account balances, with 'CASH_OUT' being the most frequent transaction type. The data shows an imbalance in fraudulent transactions, with only 0.1275% labeled as fraud.

### Visualizing the Data
Visualizations of transaction types, amounts, and account balances help identify patterns and potential indicators of fraud.

### Handling Categorical Data
One-hot encoding was applied to the 'type' column, transforming categorical data into a numeric format suitable for machine learning models.

### Dropping Identifier Columns
Columns 'nameOrig' and 'nameDest' were dropped to prevent overfitting and reduce high cardinality issues.

### Handling Imbalanced Data
The SMOTE technique was used to balance the dataset, creating synthetic samples for the minority class to enhance model training.

## Evaluation
### Logistic Regression
The model achieved high recall (89.81%) but low precision (1.35%) for fraud detection, indicating a tendency to produce false positives.

### Random Forest
This model demonstrated a good balance, with a precision of 61% and recall of 92.72%, making it effective in identifying fraud with fewer false positives.

### Decision Trees
While having high recall (94.38%), the model's precision (56%) was lower than that of Random Forest, resulting in more false positives.

### Bagging Classifier
The model had the highest recall (96.67%) but very low precision (3.37%), leading to a high number of false positives.

## Evaluation and Comparison
The performance of the models was compared using precision, recall, F1-score, and ROC-AUC score, with Random Forest emerging as the most balanced model.

## Conclusion
This study demonstrates the effectiveness of machine learning algorithms in detecting fraudulent online transactions. Random Forest stood out due to its balanced precision and recall, making it suitable for practical deployment. Future work could focus on refining these models and exploring additional features to further enhance fraud detection accuracy.
