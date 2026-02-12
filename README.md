Fake News Detection Using Natural Language Processing and Machine Learning
📌 Overview

This project focuses on detecting fake news articles using Natural Language Processing (NLP) and multiple Machine Learning algorithms. The system analyzes the textual content of news articles and predicts whether the news is Fake or Real.

The goal of this project is to demonstrate how machine learning can be applied to real-world problems such as misinformation detection.

The project was implemented in Python using Google Colab.

🎯 Problem Statement

Fake news spreads rapidly across social media platforms and online news sources. It can mislead people, influence public opinion, and create confusion.

This project aims to build a machine learning model that can automatically classify news articles based on their content.

📂 Dataset

Two datasets were used:

Fake.csv – Contains fake news articles

True.csv – Contains real news articles

Each dataset includes:

Title

Text

Subject

Date

Labels assigned:

0 → Fake News

1 → Real News

🛠️ Technologies Used

Python

Pandas

NumPy

Scikit-learn

Matplotlib

Seaborn

TF-IDF Vectorizer

⚙️ Project Workflow
1️⃣ Data Loading

The fake and real news datasets are loaded using Pandas and combined into a single dataset.

2️⃣ Data Cleaning & Preprocessing

Before training the models, the following preprocessing steps are applied:

Convert text to lowercase

Remove URLs

Remove HTML tags

Remove punctuation and special characters

Remove numbers

Drop unnecessary columns (title, subject, date)

Shuffle the dataset

This ensures that the text data is clean and ready for feature extraction.

3️⃣ Feature Extraction (TF-IDF)

Text data cannot be directly used in machine learning models. Therefore, the TF-IDF (Term Frequency – Inverse Document Frequency) technique is used to convert text into numerical feature vectors.

4️⃣ Train-Test Split

The dataset is split into:

75% Training Data

25% Testing Data

This allows us to evaluate the model performance on unseen data.

🤖 Machine Learning Models Used

Multiple supervised learning algorithms were implemented and compared:

Logistic Regression

Multinomial Naive Bayes

Support Vector Machine (Linear SVM)

Random Forest

Each model was trained on the TF-IDF features and evaluated using accuracy and classification metrics.

📊 Model Evaluation

The models were evaluated using:

Accuracy Score

Precision

Recall

F1-Score

Classification Report

Accuracy Comparison Graph

The models achieved approximately 98% accuracy, showing strong performance in distinguishing fake and real news.

A comparison graph was generated to visualize the accuracy of all models.

🧪 Manual Testing

The system allows users to manually test custom news text.

Example:

news = input("Enter news text to check: ")
manual_testing(news)


The model will output:

Fake News
or

Real News

📈 Results

Among the implemented models:

Logistic Regression performed very well

SVM also showed strong performance

Naive Bayes worked efficiently for text classification

Random Forest provided competitive results

The comparison helps identify the most suitable algorithm for fake news detection.
