# Enron Email Spam Detector

## Project Overview

Enron Email Spam Detector is a Machine Learning project that classifies emails as Spam or Ham (Not Spam). The project uses Natural Language Processing (NLP) techniques and Machine Learning algorithms to analyze email content and predict whether an email is spam or not.

---

## Objective

The objective of this project is to build a machine learning model that can automatically identify spam emails using the Enron Email Dataset.

---

## Dataset

This project uses the **Enron Email Spam Dataset**.

The dataset contains email information with the following columns:

- Subject
- Message
- Spam/Ham
- Date

Since both the email subject and message contain useful information, they were combined into a single text column before preprocessing.

---

## Technologies Used

- Python
- Pandas
- NLTK
- Scikit-learn

---

## Project Workflow

### 1. Load the Dataset

The Enron Email Spam Dataset was loaded using Pandas.

### 2. Explore the Dataset

- Checked missing values
- Removed rows with missing email messages
- Selected the required columns

### 3. Combine Subject and Message

The **Subject** and **Message** columns were combined into a single text column to improve model performance.

### 4. Text Preprocessing

The following preprocessing techniques were applied:

- Converted text to lowercase
- Removed punctuation and numbers
- Tokenized the text
- Removed stopwords

### 5. Feature Extraction

TF-IDF (Term Frequency–Inverse Document Frequency) was used to convert email text into numerical features.

### 6. Label Encoding

The target labels were converted into numeric values:

- Ham → 0
- Spam → 1

### 7. Train-Test Split

The dataset was divided into:

- 80% Training Data
- 20% Testing Data

### 8. Model Training

Two machine learning algorithms were used:

#### Multinomial Naive Bayes

A probabilistic algorithm commonly used for text classification tasks.

#### Logistic Regression

A supervised learning algorithm used for binary classification problems.

### 9. Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- F1 Score

### 10. Model Comparison

The performance of both models was compared to determine the better classifier.

### 11. Custom Email Prediction

The trained models were tested using a custom email to predict whether it was Spam or Ham.

---

## Results

| Model | Accuracy | Precision | F1 Score |
|-------|---------:|----------:|---------:|
| Naive Bayes | 98.10% | 96.44% | 98.19% |
| Logistic Regression | 99.90% | 99.80% | 99.90% |

---

## Model Comparison

Based on the evaluation metrics:

- Logistic Regression achieved higher Accuracy.
- Logistic Regression achieved higher Precision.
- Logistic Regression achieved a higher F1 Score.

Therefore, **Logistic Regression performed better than Naive Bayes on the Enron Email Dataset.**

---

## Sample Prediction

### Input Email

```
Congratulations! You have won a free iPhone.
Click the link below to claim your prize.
```

### Prediction

**Spam**

---

## Conclusion

In this project, email subjects and messages were combined and preprocessed using Natural Language Processing (NLP) techniques. The processed text was converted into numerical features using TF-IDF, and two machine learning models were trained and evaluated.

Among the two models, **Logistic Regression achieved the best performance** with an accuracy of approximately **99.90%**, making it the most effective model for email spam detection on the Enron Email Dataset.

---

## Project developed by

**Rupali Rathore**

B.Tech (Information Technology)
