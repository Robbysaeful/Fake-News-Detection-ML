# 📰 Fake News Detection Using Natural Language Processing and Machine Learning

## 📌 Overview

This project implements a Fake News Detection system using Natural Language Processing (NLP) and multiple Machine Learning algorithms.  
The system analyzes news article text and predicts whether the news is **Fake** or **Real**.

The project is developed using **Python** and executed in **Google Colab**.

---

## 🎯 Problem Statement

Fake news spreads rapidly across social media platforms and online news websites, influencing public opinion and creating misinformation.

The goal of this project is to build a machine learning model that can automatically classify news articles based on their textual content.

---

## 📂 Dataset

Two datasets are used in this project:

- `Fake.csv` – Contains fake news articles  
- `True.csv` – Contains real news articles  

Each dataset contains the following columns:

- Title  
- Text  
- Subject  
- Date  

### Labels:
- `0` → Fake News  
- `1` → Real News  

---

## 🛠️ Technologies Used

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  
- TF-IDF Vectorizer  

---

## ⚙️ Project Workflow

### 1️⃣ Data Loading
The fake and real news datasets are loaded using Pandas and merged into a single dataset.

### 2️⃣ Data Preprocessing
The following preprocessing steps are applied:

- Convert text to lowercase  
- Remove URLs  
- Remove HTML tags  
- Remove punctuation and numbers  
- Drop unnecessary columns (title, subject, date)  
- Shuffle the dataset  

### 3️⃣ Feature Extraction
TF-IDF (Term Frequency – Inverse Document Frequency) is used to convert text data into numerical vectors.

### 4️⃣ Train-Test Split
The dataset is split into:
- 75% Training Data  
- 25% Testing Data  

---

## 🤖 Machine Learning Models Used

The following supervised learning algorithms were implemented and compared:

- Logistic Regression  
- Multinomial Naive Bayes  
- Support Vector Machine (Linear SVM)  
- Random Forest  

---

## 📊 Model Evaluation

Models were evaluated using:

- Accuracy Score  
- Precision  
- Recall  
- F1-Score  
- Classification Report  
- Accuracy Comparison Graph  

The best-performing model achieved approximately **98% accuracy**.

---

## 📈 Model Comparison

All models were compared based on their accuracy scores and visualized using a bar chart.

Example comparison:

