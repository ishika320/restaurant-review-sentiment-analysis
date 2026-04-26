
# Restaurant Review Sentiment Analysis using NLP and Machine Learning

## Project Overview

This project focuses on analyzing restaurant customer reviews using Natural Language Processing (NLP) and Machine Learning techniques. The system automatically classifies customer feedback into two categories:

- Complaint
- Positive Aspect

The goal of this project is to help restaurants quickly identify customer satisfaction levels and common service issues by analyzing large volumes of review data.

---

## Problem Statement

Online restaurant platforms generate massive amounts of customer feedback through text reviews. Manually analyzing thousands of reviews is time-consuming and inefficient.

Therefore, this project aims to develop an automated sentiment classification system that can analyze restaurant reviews and identify whether the feedback represents a complaint or a positive aspect.

---

## Objectives

- Analyze customer feedback for restaurants
- Identify common complaints and positive aspects
- Build a machine learning model for sentiment classification
- Compare multiple machine learning algorithms
- Evaluate model performance using statistical metrics

---

## Dataset Information

The dataset used in this project consists of restaurant customer reviews collected from an online platform.

### Dataset Features

| Feature | Description | Data Type |
|--------|-------------|----------|
| Review | Customer review text | String |
| Rating | Star rating (1–5) | Integer |
| Sentiment | Complaint or Positive Aspect | String |
| Clean Review | Preprocessed review text | String |

### Dataset Statistics

- Total Reviews: 12,098
- Positive Reviews: 10,881
- Complaint Reviews: 1,217
- Dataset Type: Text Data
- Problem Type: Binary Classification

---

## Technologies and Libraries Used

### Programming Language

- Python

### Libraries

- pandas
- numpy
- matplotlib
- seaborn
- nltk
- scikit-learn
- wordcloud

---

## Project Workflow

1. Data Collection  
2. Data Preprocessing  
3. Feature Extraction  
4. Model Training  
5. Model Evaluation  
6. Prediction  

---

## Data Preprocessing Steps

The following preprocessing techniques were applied to clean and prepare the text data:

- Convert text to lowercase
- Remove punctuation and special characters
- Remove stop words
- Remove short reviews
- Handle missing values
- Create sentiment labels

Example:

Original text:

The FOOD was AMAZING!!!

Cleaned text:

food amazing

---

## Feature Extraction

The TF-IDF (Term Frequency–Inverse Document Frequency) technique was used to convert text into numerical form.

TF-IDF assigns higher importance to meaningful words and reduces the impact of common words.

Formula:

TF = Number of times word appears / Total words

IDF = log(Total documents / Documents containing word)

TF-IDF = TF × IDF

---

## Machine Learning Models Used

Three machine learning algorithms were implemented and compared.

### 1. Logistic Regression

A statistical model used for binary classification. It predicts the probability that a review belongs to a specific class.

### 2. Naive Bayes

A probabilistic classifier based on Bayes' theorem. It assumes independence between features and works efficiently with text data.

### 3. Support Vector Machine (SVM)

A powerful classification algorithm that finds the optimal boundary separating classes. It performs well on high-dimensional text data.

---

## Handling Imbalanced Dataset

The dataset was imbalanced because the number of positive reviews was higher than complaint reviews.

To address this issue, the following techniques were applied:

- Undersampling
- Class weighting
- Stratified train-test split

These methods improved model fairness and classification performance.

---

## Evaluation Metrics

The performance of the models was evaluated using the following metrics:

- Accuracy
- Precision
- Recall (Sensitivity)
- F1 Score
- Specificity
- False Positive Rate (FPR)
- False Negative Rate (FNR)
- Negative Predictive Value (NPV)
- False Discovery Rate (FDR)
- Matthews Correlation Coefficient (MCC)
- Confusion Matrix

---

## Model Performance

| Metric | Logistic Regression | Naive Bayes | SVM |
|-------|--------------------|------------|-----|
| Accuracy | 0.949 | 0.932 | 0.976 |
| Precision | 0.947 | 0.930 | 0.987 |
| Recall | 0.999 | 0.999 | 0.993 |
| F1 Score | 0.972 | 0.964 | 0.987 |
| MCC | 0.683 | 0.549 | 0.865 |

---

## Best Model

Support Vector Machine (SVM) achieved the highest performance across most evaluation metrics.

Best Model Accuracy:

97.6%

Therefore, SVM was selected as the final model for restaurant review sentiment classification.

---

## Example Prediction

Input Review:

Food was amazing and staff was friendly

Output:

Positive Aspect

---

Input Review:

Service was slow and food was cold

Output:

Complaint

---

## Visualizations Included

The project includes the following visualizations:

- Sentiment Distribution Graph
- Model Comparison Graph
- Confusion Matrix
- Word Frequency Analysis
- Hyperparameter Tuning Graph

---

## Project Structure

restaurant-review-sentiment-analysis/
│
├── dataset/
│   └── Yelp_Restaurant_Reviews.csv
│
├── notebook/
│   └── sentiment_analysis.ipynb
│
├── requirements.txt
│
└── README.md

---

## How to Run the Project

Step 1:

Install required libraries

Step 2:

Run the notebook

---

## Applications

This system can be used in:

- Restaurant feedback analysis
- Customer satisfaction monitoring
- Business decision making
- Online review analysis
- Sentiment analysis systems

---

## Future Improvements

- Use deep learning models such as LSTM or BERT
- Deploy the model as a web application
- Add real-time review analysis
- Improve handling of sarcasm and slang

---

## Author

Ishika   
B.Tech Computer Science Engineering  
Manipal University Jaipur  

---

## References

- Scikit-learn Documentation  
https://scikit-learn.org

- NLTK Documentation  
https://www.nltk.org

- Python Documentation  
https://docs.python.org

- Kaggle Dataset  
https://www.kaggle.com

- Han, J., Kamber, M., & Pei, J.  
Data Mining: Concepts and Techniques

- Jurman, G., Riccadonna, S., & Furlanello, C.  
Comparison of MCC and F1 Score for Classification
