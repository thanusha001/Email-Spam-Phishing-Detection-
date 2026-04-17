# 📧 Spam & Phishing Email Detection using Machine Learning

## 📌 Overview
This project implements a Machine Learning-based solution to detect **spam and phishing emails**. It uses Natural Language Processing (NLP) techniques along with a **Naïve Bayes classifier** to classify messages as either **legitimate (ham)** or **malicious (spam/phishing)**.

## 🚀 Live Demo
👉 https://huggingface.co/spaces/thanupage/email_spam_and_phishing_detection

## 🚀 Features
- Spam vs Legitimate email classification
- Text preprocessing and cleaning
- Feature extraction using TF-IDF (unigrams + bigrams)
- Model training using Multinomial Naïve Bayes
- Performance evaluation (accuracy, confusion matrix, classification report)
- Model saving and reuse
- Custom prediction for new inputs

## 🛠️ Tech Stack
- Python  
- Pandas, NumPy  
- Scikit-learn  
- NLTK  
- Matplotlib, WordCloud  
- Joblib  

## 📂 Workflow

### 1. Data Loading
- Load dataset from CSV
- Identify text and label columns

### 2. Preprocessing
- Convert text to lowercase  
- Remove URLs, HTML tags, emails, numbers, punctuation  
- Remove stopwords  
- Apply stemming  

### 3. Train-Test Split
- 75% training / 25% testing  
- Stratified sampling  

### 4. Model Pipeline
- TF-IDF Vectorizer (n-grams: 1,2)  
- Multinomial Naïve Bayes  

### 5. Evaluation
- Accuracy Score  
- Confusion Matrix  
- Classification Report  

### 6. Model Saving
- Save trained model using Joblib  

### 7. Prediction
```python
sample = "Congratulations! You have won a lottery."
prediction = model.predict([sample])
