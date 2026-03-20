# 🚀 Reddit Virality Predictor

## 📌 Overview

This project predicts whether a Reddit post will go **viral** using a combination of:

* 📊 Early engagement signals (upvotes, comments)
* 🧠 Sentiment analysis of text content

The goal is to understand **what drives online engagement** and build a model that can make predictions **as early as possible after posting**.

---

## 🎯 Objectives

* Predict viral Reddit posts using machine learning
* Combine **text sentiment** with **early attention features**
* Analyse patterns that influence post popularity

---

## 📊 Dataset

Data is collected using the Reddit API via `PRAW`.

Each post includes:

* Title
* Body text
* Upvotes (score)
* Number of comments
* Timestamp

Subreddits used:

* r/technology
* r/gaming
* r/worldnews

---

## ⚙️ Methodology

### 1. Data Collection

* Fetch Reddit posts using PRAW
* Collect metadata and textual content

### 2. Data Preprocessing

* Clean text (remove links, punctuation, stopwords)
* Merge title and body
* Handle missing values

### 3. Feature Engineering

#### 🔹 Text Features

* Sentiment score (VADER)
* Text length
* TF-IDF vectors

#### 🔹 Early Attention Features

* Upvotes
* Comment count
* Post age (hours)

---

### 4. Target Variable

Posts are classified as:

* **Viral (1)** → Top 20% by upvotes
* **Not Viral (0)** → Remaining posts

---

### 5. Models Used

* Logistic Regression
* Random Forest
* XGBoost

---

### 6. Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1 Score

---

## 📈 Key Insights

* Early engagement signals strongly influence virality
* Sentiment alone is not sufficient
* Combining **text + engagement features** improves prediction performance

---

## 🚀 Future Improvements

* Real-time prediction system
* More subreddits and larger dataset
* Deep learning models (BERT, LSTM)
* Interactive dashboard using Streamlit

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* NLTK (VADER)
* XGBoost
* Matplotlib / Seaborn
* PRAW (Reddit API)

---

## 📂 Project Structure

```
reddit-virality-predictor/
│
├── data/
├── notebooks/
├── src/
├── app/
├── README.md
└── requirements.txt
```

---

## 💡 How to Run

1. Clone the repository:

```
git clone https://github.com/your-username/reddit-virality-predictor.git
```

2. Install dependencies:

```
pip install -r requirements.txt
```

3. Run the notebook:

```
notebooks/reddit_analysis.ipynb
```

---

## 🎯 Project Motivation

This project was developed to explore how **early attention dynamics and sentiment** influence content virality on social media platforms.

It is designed as a **research-oriented project** suitable for:

* Data Science portfolios
* PhD applications
* Machine Learning case studies

---

## 🤝 Contributing

Feel free to fork this repo and contribute!

---

## ⭐ If you like this project

Give it a star ⭐ on GitHub!
