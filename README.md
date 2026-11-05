# Food-Delivery-Sentiment-Analysis
A machine learning project that predicts customer sentiment (Positive, Negative, Neutral) based on food temperature, freshness, packaging quality, and food condition.  Compares five classification algorithms using Accuracy, Precision, Recall, and Weighted F1 Score to identify the best-performing model.

Predicting customer sentiment (**Positive / Negative / Neutral**) from food quality using five machine learning algorithms.

---

## 📌 Project Overview

Food delivery customers judge a service by the condition in which the food arrives. This project analyses food quality using machine learning and predicts customer sentiment as **Positive**, **Negative**, or **Neutral** based on four inputs: food temperature, food freshness, packaging quality, and food condition.

Five classification algorithms are trained and compared, and the best-performing one is identified using the Weighted F1 Score.

---

## 🎯 Objectives

- To analyse food quality.
- To classify customer sentiment as Positive, Negative, or Neutral.
- To compare five machine learning algorithms and find the best one.

---

## ✨ Features

- Works on a dataset of **10,000 records**.
- Predicts sentiment from four food-quality inputs: Food Temperature, Food Freshness, Packaging Quality, Food Condition.
- Converts the 1–5 customer satisfaction rating into sentiment classes:
  - 1–2 → Negative
  - 3 → Neutral
  - 4–5 → Positive
- Compares five algorithms side by side using Accuracy, Precision, Recall, and Weighted F1 Score.
- Includes graphs for sentiment distribution and algorithm comparison.

### Dataset Summary

| Item | Details |
| --- | --- |
| Total records | 10,000 |
| Target variable | Customer Satisfaction |
| Features | Food Temperature, Food Freshness, Packaging Quality, Food Condition |
| Negative | 4,051 customers |
| Positive | 3,928 customers |
| Neutral | 2,021 customers |
| Train / Test split | 8,000 / 2,000 (80:20) |

---

## 🤖 Machine Learning

### Algorithms Used

| Algorithm | Purpose |
| --- | --- |
| Logistic Regression | Classifies customer sentiment |
| Naive Bayes | Predicts sentiment using probability |
| KNN (K-Nearest Neighbors) | Classifies based on nearest data points |
| SVM (Support Vector Machine) | Separates different sentiment classes |
| Random Forest | Uses multiple decision trees for prediction |

### Evaluation Metrics

- **Accuracy:** overall correct predictions.
- **Precision:** measures prediction correctness.
- **Recall:** measures correctly identified records.
- **Weighted F1 Score:** balances precision and recall.

### Results

| Classifier | Accuracy | Precision | Recall | F1 Score |
| --- | --- | --- | --- | --- |
| **KNN** | 36.10% | 36.12% | 36.10% | **35.92%** |
| Naive Bayes | 40.00% | 31.93% | 40.00% | 34.92% |
| SVM | 33.40% | 36.09% | 33.40% | 33.97% |
| Logistic Regression | 33.00% | 34.35% | 33.00% | 33.50% |
| Random Forest | 32.80% | 35.27% | 32.80% | 33.46% |

### 🏆 Best Algorithm: KNN

- Achieved the highest Weighted F1 Score of **35.92%**.
- Provides a better balance between Precision and Recall.
- Predicts sentiment by identifying similar food-quality records.

---

## 🛠️ Technologies Used

| Category | Tools |
| --- | --- |
| Language | Python |
| Libraries | Pandas, NumPy, Scikit-learn |
| Visualization | Matplotlib, Seaborn |
| Environment | Jupyter Notebook / Google Colab |
| Version control | Git and GitHub |

---

## 📁 Project Structure

```
food-delivery-sentiment-analysis/
├── README.md                          # Project documentation
├── requirements.txt                   # Python dependencies
├── data/
│   └── food_delivery_reviews.csv      # Dataset (10,000 records)
├── notebooks/
│   └── sentiment_analysis.ipynb       # Complete code
├── results/
│   ├── sentiment_distribution.png     # Graph 1: sentiment counts
│   └── f1_comparison.png              # Graph 2: algorithm F1 scores
└── docs/
    └── Case_Study_Slides.pptx         # Presentation
```

---

## 🔄 Machine Learning Workflow

1. **Data collection:** load the food delivery dataset (10,000 records).
2. **Data cleaning and preprocessing:** handle missing values and prepare the features.
3. **Sentiment labelling:** map ratings to Negative (1–2), Neutral (3), Positive (4–5).
4. **Train–test split:** 80:20 split, giving 8,000 training and 2,000 testing records.
5. **Model training:** train Logistic Regression, Naive Bayes, KNN, SVM, and Random Forest.
6. **Model testing:** predict sentiment on the 2,000 test records.
7. **Evaluation:** calculate Accuracy, Precision, Recall, and Weighted F1 Score.
8. **Model comparison:** compare all five classifiers.
9. **Best model selection:** choose KNN, which has the highest Weighted F1 Score.

---
---

## 🚀 Future Enhancements

- Improve accuracy by adding more features such as delivery time, distance, and price.
- Apply hyperparameter tuning (for example GridSearchCV) to every model.
- Handle the class imbalance, since Neutral reviews are far fewer than the others.
- Try advanced models such as XGBoost, or deep learning models.
- Add text-based review analysis using NLP.
- Build a web app where a user enters food-quality details and gets the predicted sentiment.

---

## 📊 Project Status

**Completed**: model training, evaluation, comparison, and result visualization are done. The project is open to the enhancements listed above.
