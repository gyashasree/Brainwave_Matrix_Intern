
# Fake News Detection

Overview

The rise of misinformation and fake news is a significant concern in today's world. This project aims to tackle this issue using machine learning techniques to classify news articles as either true or fake. The model is trained on a labeled dataset, which includes both legitimate and fake news articles, to develop a reliable fake news detection system.

Dataset

The dataset used in this project consists of two CSV files:

True.csv: Contains legitimate news articles.
Fake.csv: Contains fake or misleading news articles.
The datasets have been labeled:
Class 0: Fake news.
Class 1: Real news.
Both datasets include text data representing news articles, and the project involves preprocessing this data for model training and evaluation.

Features

Text: The content of the news articles.
Class: The target variable where 0 indicates fake news and 1 indicates real news.

Techniques Used

Data Preprocessing
Handled missing values, if any.
Removed unnecessary characters such as punctuation using regular expressions.
Performed basic text cleaning to prepare the data for model input.


Model Selection

Used the train_test_split function to split the data into training and testing sets.
Employed various machine learning algorithms, including:
Logistic Regression
Naive Bayes
Support Vector Machines (SVM)
Random Forest Classifier
Evaluated model performance based on accuracy and classification metrics.

Evaluation Metrics

The performance of the models is evaluated using the following metrics:Accuracy,
Precision,
Recall,
F1-score,
Confusion Matrix.

Model Implementation

Data Preprocessing:Combined the two datasets (fake and true news) into a single dataframe.
Cleaned and preprocessed the text data by removing special characters and unnecessary punctuation.
Split the dataset into training and testing subsets (80% training, 20% testing).

Model Training:

Trained multiple classification models on the preprocessed text data.
Fine-tuned the models using hyperparameter optimization to improve performance.

Model Evaluation:

Evaluated model accuracy and classification metrics such as precision, recall, and F1-score.
Plotted confusion matrices and classification reports for better understanding of the model's effectiveness.

Results

The following metrics were used to evaluate the model's performance:

Accuracy: Measures the proportion of correctly classified articles.
Precision: Indicates the percentage of correctly identified fake news articles.
Recall: Reflects the model’s ability to detect actual fake news.
F1-score: A harmonic mean of precision and recall.
The results showed that the selected machine learning algorithms were effective in distinguishing between real and fake news articles.
