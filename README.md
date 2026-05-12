# Review Sentiment Analysis Using NLP & Machine Learning

## Project Overview

This project presents an end-to-end **Sentiment Analysis and Review Classification System** using **Natural Language Processing (NLP)** and **Machine Learning** in Python.

The objective of the project is to classify customer reviews into **positive** or **negative sentiments**, helping businesses understand customer opinions and improve decision-making.

The project demonstrates a complete NLP workflow including:

- Text preprocessing
- Feature extraction using TF-IDF
- Sentiment classification
- Model comparison
- Model evaluation
- Prediction system
- Review moderation logic

---

## Dataset Information

The dataset contains **4,321 customer reviews** and corresponding sentiment labels.

### Dataset Features

| Column | Description |
|--------|-------------|
| `review` | Customer review text |
| `class` | Sentiment label (0 = Negative, 1 = Positive) |

### Dataset Characteristics

- Total Records: **4,321**
- Positive Reviews: **2,989**
- Negative Reviews: **1,332**
- Binary Classification Problem

---

## Project Objectives

The project aims to answer the following questions:

- Can customer reviews be automatically classified as positive or negative?
- Which machine learning model performs better for sentiment analysis?
- How effective is TF-IDF for representing review text?
- Can sentiment classification support automated moderation systems?

---

## Text Preprocessing

Before model training, several preprocessing steps were applied to improve text quality and consistency.

### Preprocessing Steps

- Lowercase conversion
- Removal of punctuation
- Removal of special characters
- Stopword removal
- Text cleaning
- Empty review removal

These steps help improve model performance by reducing noise in textual data.

---

## Feature Engineering

### TF-IDF Vectorization

The textual reviews were transformed into numerical features using:

```python
TfidfVectorizer()
```

TF-IDF (**Term Frequency–Inverse Document Frequency**) helps identify important words in reviews while reducing the importance of overly common words.

---

## Machine Learning Models

The following models were implemented and compared:

### 1. Logistic Regression
A strong baseline model for text classification tasks.

### 2. Naive Bayes
A probabilistic machine learning algorithm commonly used in NLP classification problems.

---

## Model Evaluation

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### Best Model Performance

**Logistic Regression Accuracy: ~92%**

The model demonstrated strong predictive performance, particularly for identifying positive sentiment reviews.

However, performance on negative reviews highlighted the importance of considering **Recall and F1-score**, not only overall accuracy.

---

## Prediction Demo

The project includes a prediction system capable of classifying new unseen reviews.

### Example:

**Input Review**

```text
The service was excellent and fast
```

**Prediction**

```text
Positive Review
```

---

## Moderation Logic

A simple moderation layer was implemented to help flag potentially problematic reviews.

The system combines:

- Sentiment prediction
- Abusive keyword detection

This demonstrates how sentiment analysis can support automated review moderation.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- NLTK
- TF-IDF Vectorizer
- Logistic Regression
- Naive Bayes
- Matplotlib
- Seaborn
- Google Colab

---

## Repository Structure

```text
review-sentiment-analysis/
│── Review_Sentiment_Model.ipynb
│── TestReviews.csv
│── README.md
```

---

## Key Findings

1. Logistic Regression outperformed Naive Bayes for sentiment classification.

2. TF-IDF effectively transformed text into meaningful numerical features.

3. The model performed strongly overall with approximately **92% accuracy**.

4. Negative reviews were slightly harder to classify than positive reviews, highlighting class imbalance challenges.

5. Review moderation can be enhanced through sentiment classification and keyword detection.

---

## Conclusion

This project demonstrates a complete **end-to-end NLP and sentiment analysis workflow** using Python and machine learning.

The work highlights practical skills in:

- Text preprocessing
- Feature engineering
- Machine learning model building
- Model evaluation
- Sentiment classification
- NLP problem-solving

The project also demonstrates how sentiment analysis can be applied to real-world customer feedback and moderation systems.

---

## Author

**Righteous Udurume**  
Data Analyst | Data Scientist | Aspiring Data Engineer

Passionate about transforming raw data into actionable insights through **data analysis, machine learning, and data-driven problem solving**.

**Skills:**  
Python • SQL • Data Analysis • Data Visualization • Machine Learning • NLP • Exploratory Data Analysis • Power BI
