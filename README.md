# Enron Email Spam Detector

## Project Overview

Enron Email Spam Detector is a Machine Learning project that classifies emails as Spam or Ham (Not Spam). The project uses Natural Language Processing (NLP) techniques and Machine Learning algorithms to analyze email content and predict whether an email is spam or not.

---

## Objective

The objective of this project is to build a machine learning model that can automatically classify emails as Spam or Ham using the Enron Email Dataset.

---

## Dataset

This project uses the **Enron Email Spam Dataset**.

The dataset contains the following columns:

* Subject
* Message
* Spam/Ham
* Date

The **Subject** and **Message** columns were combined into a single text column before preprocessing.

> **Note:** The dataset is included in this repository as a ZIP file (`enron_spam_data.zip`). Please extract the ZIP file before running the notebook.

---

## Technologies Used

* Python
* Pandas
* NLTK
* Scikit-learn

---

## Project Workflow

### 1. Load the Dataset

The Enron Email Spam Dataset was loaded using Pandas.

### 2. Explore the Dataset

* Checked missing values
* Removed rows with missing email messages
* Selected the required columns

### 3. Combine Subject and Message

The Subject and Message columns were merged into a single text column.

### 4. Text Preprocessing

The following preprocessing steps were applied:

* Converted text to lowercase
* Removed punctuation and numbers
* Tokenized the text
* Removed English stopwords

### 5. Feature Extraction

TF-IDF (Term Frequency–Inverse Document Frequency) was used to convert text into numerical features.

### 6. Label Encoding

The target labels were encoded as:

* Ham → 0
* Spam → 1

### 7. Train-Test Split

The dataset was divided into:

* 80% Training Data
* 20% Testing Data

### 8. Model Training

Two machine learning algorithms were trained:

* Multinomial Naive Bayes
* Logistic Regression

### 9. Model Evaluation

The models were evaluated using:

* Accuracy
* Precision
* F1 Score

### 10. Model Comparison

Both models were compared based on their evaluation metrics.

### 11. Custom Email Prediction

The trained models were tested using a custom email for prediction.

---

## Results

| Model               | Accuracy | Precision | F1 Score |
| ------------------- | -------: | --------: | -------: |
| Naive Bayes         |   98.10% |    96.44% |   98.19% |
| Logistic Regression |   99.90% |    99.80% |   99.90% |

---

## Model Comparison

The comparison shows that **Logistic Regression** achieved better performance than **Naive Bayes** on the Enron Email Dataset.

* Higher Accuracy
* Higher Precision
* Higher F1 Score

Therefore, **Logistic Regression** was selected as the better model for this project.

---

## Sample Prediction

### Input Email

```
Congratulations! You have won a free iPhone.
Click the link below to claim your prize.
```

### Model Output

```
Naive Bayes Prediction : Ham
Logistic Regression Prediction : Ham
```

> The prediction shown above is the actual output generated during project execution.

---

## Conclusion

This project demonstrates how Natural Language Processing (NLP) and Machine Learning can be used for email spam detection. Email subjects and messages were combined, preprocessed, and converted into TF-IDF features before training the models.

Among the two algorithms, **Logistic Regression** achieved the best performance with an accuracy of **99.90%**, making it the most effective model for the Enron Email Dataset.

---

## Project Structure

```
Enron-Email-Spam-Detector/
│── enron-email-spam-detector.ipynb
│── enron_spam_data.zip
│── README.md
```

---

## Project developed by

**Rupali Rathore**

B.Tech (Information Technology)
