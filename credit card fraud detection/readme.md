# Credit Card Fraud Detection
Overview

Credit card fraud is a serious issue that impacts consumers and financial institutions worldwide. This project aims to detect fraudulent transactions by leveraging machine learning techniques. The model is trained on a labeled dataset consisting of both legitimate and fraudulent transactions, and it strives to accurately distinguish between the two.

Dataset:

The dataset used in this project consists of anonymized transaction records labeled as either fraud or legitimate:

Features: Various anonymized attributes related to credit card transactions.
Class: The target variable where 0 represents a legitimate transaction and 1 indicates a fraudulent transaction.
The dataset is highly imbalanced, with a much smaller proportion of fraudulent transactions compared to legitimate ones. Techniques to handle this imbalance are applied during model training and evaluation.

Features:

Transaction Features: Includes anonymized features (V1, V2, ..., V28) representing transaction-specific information.
Time: The time elapsed between this transaction and the first transaction in the dataset.
Amount: The monetary value of the transaction.
Class: The target variable where 0 represents non-fraudulent transactions and 1 represents fraudulent transactions.

Techniques Used:

Data Preprocessing:

Handled missing values, if any.
Scaled the features using appropriate scaling techniques to handle large discrepancies between transaction amounts.
Performed data balancing to address the highly imbalanced dataset using techniques like undersampling or SMOTE (Synthetic Minority Oversampling Technique).

Model Selection:

The dataset was split into training and testing sets using train_test_split. Several machine learning algorithms were applied, including:

Logistic Regression,
Decision Trees,
Random Forest,
XGBoost,
Support Vector Machines (SVM).
Each model’s performance was evaluated and fine-tuned using hyperparameter optimization techniques to improve their accuracy in identifying fraudulent transactions.

Evaluation Metrics:

The performance of the models was evaluated using several key metrics:

Accuracy: The proportion of correctly classified transactions.
Precision: The percentage of correctly identified fraudulent transactions among all predicted frauds.
Recall: The model's ability to detect actual frauds.
F1-score: The harmonic mean of precision and recall, providing a balance between both metrics.
Confusion Matrix: Visual representation of the true positive, true negative, false positive, and false negative predictions.

Model Implementation:

Data Preprocessing:
Scaled and normalized the features for better model performance.
Split the dataset into an 80% training set and 20% testing set.

Model Training:

Trained multiple models on the preprocessed data.
Optimized hyperparameters to improve each model's performance.
Implemented techniques to handle data imbalance, such as class weighting and resampling methods.

Model Evaluation:

Evaluated the models using metrics like accuracy, precision, recall, and F1-score.
Generated confusion matrices and classification reports to better understand each model's strengths and weaknesses.

Results

The model evaluation revealed the following:

Accuracy: The percentage of correctly classified transactions (both legitimate and fraudulent).
Precision: The proportion of correctly predicted fraudulent transactions out of all predicted frauds.
Recall: The model's ability to correctly identify actual frauds.
F1-Score: A balanced measure of precision and recall.
The results indicated that the machine learning models employed were effective in distinguishing between legitimate and fraudulent transactions. Handling the imbalanced dataset was key to improving the performance of the models, ensuring that the models are capable of detecting fraud without generating excessive false positives.
