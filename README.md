# Fake News Detection using Machine Learning

This project is a simple implementation of a **Fake News Detection system** using **Machine Learning**.  
It analyzes news articles and predicts whether the given news is **Fake** or **Real** using text data.

The model is built using **Logistic Regression** and **TF-IDF Vectorization**, and the project is implemented in **Python using Google Colab**.

---

## About the Project
Fake news spreads very fast on social media and news platforms.  
The goal of this project is to use **Natural Language Processing (NLP)** and **Machine Learning** to automatically identify fake news based on the content of the article.

---

## Dataset
Two datasets are used in this project:
- `Fake.csv` – contains fake news articles
- `True.csv` – contains real news articles

Each dataset includes:
- Title
- Text
- Subject
- Date

Labels:
- `0` → Fake News  
- `1` → Real News  

---

## Tools & Technologies Used
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  
- TF-IDF Vectorizer  
- Logistic Regression  

---

## Data Preprocessing
Before training the model, the following preprocessing steps are applied:
- Convert text to lowercase
- Remove URLs and HTML tags
- Remove punctuation and numbers
- Remove unnecessary columns (`title`, `subject`, `date`)
- Shuffle the dataset

---

## Model Used
- **Algorithm:** Logistic Regression  
- **Feature Extraction:** TF-IDF Vectorizer  
- **Train-Test Split:** 75% training, 25% testing  

---

## Model Performance
The model performs very well on the dataset:
- **Accuracy:** ~98%
- High precision and recall for both fake and real news

---

## Manual Testing
The project also allows manual testing by entering your own news text.

Example:
```python
news = "Enter your news text here"
manual_testing(news)
