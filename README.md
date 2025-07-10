COMPANY : CODTECH IT SOLUTIONS

NAME: BHAVYA DIGRA

INTERN ID: CITS0D698

DOMAIN:DATA ANALYST

DURATION: 4 WEEKS

MENTOR:NEELA SANTOSH

# 📊 Sentiment Analysis using Natural Language Processing (NLP)

---

## 📝 Project Overview

This project is submitted as part of **Task 4** of the **CODTECH Internship Program**, which focuses on applying **Natural Language Processing (NLP)** techniques to perform **sentiment analysis** on textual data such as tweets and reviews.

The goal of this task was to clean and preprocess raw textual data, build a machine learning model that can classify sentiments (positive or negative), and evaluate its performance based on relevant metrics. The entire workflow, from data cleaning to model evaluation, has been implemented using Python in a Jupyter Notebook.

As a second-year engineering student with a growing interest in data science and machine learning, this task gave me real-world exposure to building a complete data-driven project from scratch.

---

## 📌 Problem Statement

> “Build a sentiment analysis system using machine learning and NLP techniques that can classify whether a given review or tweet expresses a positive or negative sentiment.”

The dataset provided was a version of the **Sentiment140 Twitter dataset**, which consists of 1.6 million tweets labeled with sentiment polarity:
- **0** → Negative sentiment
- **4** → Positive sentiment

---

## ⚙️ Project Workflow

### 1. **Importing Libraries**
Utilized powerful libraries such as:
- `pandas`, `numpy` for data manipulation
- `nltk` for text preprocessing
- `sklearn` for machine learning and evaluation
- `matplotlib`, `seaborn` for visualizations

---

### 2. **Data Loading and Cleaning**
- Loaded the dataset using `pandas.read_csv()` with proper encoding and skipped bad lines.
- The dataset had 6 columns: `target`, `id`, `date`, `flag`, `user`, and `text`. I retained only `target` and `text` for sentiment classification.

---

### 3. **Preprocessing**
Using NLTK:
- Removed URLs, non-letter characters, and converted text to lowercase.
- Removed stopwords like "the", "is", etc.
- Applied stemming to reduce words like “loved”, “loving” to their root “love”.

This drastically cleaned the text and reduced noise for the model.

---

### 4. **Vectorization**
Used `CountVectorizer` from Scikit-learn to convert text into numerical format using Bag-of-Words (BoW) with 5000 most frequent words.

---

### 5. **Model Training**
Trained a **Logistic Regression** model using the processed and vectorized data:
- Dataset: ~1.6M samples (800K positive, 800K negative)
- Train-test split: 80/20 using stratification to maintain class balance

---

### 6. **Model Evaluation**
- Achieved an accuracy of **76.77%**
- Confusion Matrix and classification report were generated
- Plotted confusion matrix using `seaborn.heatmap` for clear visualization

---

## ✅ Results Summary

| Metric          | Value         |
|----------------|---------------|
| Accuracy        | 76.77%        |
| F1-Score (Macro)| 77%           |
| Dataset Size    | 1.6 Million Tweets |
| Model           | Logistic Regression |

---

## 📈  Visualization

<img width="1019" height="702" alt="image" src="https://github.com/user-attachments/assets/0368511a-6671-4cb2-8ca3-bb4b34ab221e" />
<img width="890" height="754" alt="image" src="https://github.com/user-attachments/assets/1ed1437f-0076-4966-9474-b0e521440bc7" />

This plot helped me visually interpret how many tweets were correctly and incorrectly classified as positive or negative.

---

## 🌍 Real Life Applications of Sentiment Analysis

- **Customer Feedback Monitoring**: Brands use it to gauge public sentiment about their products or services.
- **Social Media Monitoring**: Used in elections, product launches, and crisis management to track public reactions on platforms like Twitter.
- **Stock Market Prediction**: Investors analyze sentiment from news articles or tweets to make informed decisions.
- **E-commerce**: Sites like Amazon use it to filter fake reviews or highlight genuine customer feedback.
- **Chatbots & Virtual Assistants**: To interpret user mood and improve human-computer interactions.

Through this project, I realized how powerful even basic machine learning models can be when combined with proper data cleaning and NLP techniques.

---

## 💡 Learnings

This was my **first end-to-end NLP project** using a real-world dataset. I learned:
- How to clean unstructured data (tweets are messy!)
- Why text preprocessing is critical before vectorization
- How to tune and evaluate models using F1-score and confusion matrix
- The value of visualization in storytelling and interpretation
- Practical usage of libraries like `nltk`, `sklearn`, and `seaborn`
