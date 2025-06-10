# Fake News Detection using Machine Learning

This project predicts whether a news article is **fake or real** based on its textual content and metadata using a **Logistic Regression** classifier. Built using Scikit-learn and real Twitter data.

![Python](https://img.shields.io/badge/Python-3.10-blue.svg)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.3.0-orange)

## Overview

- Input: News article title, source domain, tweet count
- Output: Prediction — Real or Fake
- Model: Logistic Regression
- Vectorizer: TF-IDF on the article title
- Encoders: One-Hot Encoding for domain; raw numeric input for tweet count

## Dataset Description

The dataset used is from **FakeNewsNet**, a comprehensive fake news repository including text, source, and social engagement data.

### Features

| Feature         | Description                                         |
|----------------|-----------------------------------------------------|
| `title`         | Headline/title of the news article                 |
| `source_domain` | Domain name from where the article originated      |
| `tweet_num`     | Number of tweets that shared this news article     |

### 🎯 Target Variable

| Variable | Description          |
|----------|----------------------|
| `real`   | 1 = Real news, 0 = Fake news |

> 📎 [FakeNewsNet](https://github.com/KaiDMML/FakeNewsNet) is the source for this dataset.

## Technologies Used

- Python
- pandas, numpy
- scikit-learn

## Model Evaluation

- Logistic Regression accuracy: ~ 87%
