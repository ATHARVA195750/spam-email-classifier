# Spam Email Classifier

A machine learning model that classifies SMS messages as spam or legitimate (ham).

## Results
- Accuracy: 98.47%
- Precision (spam): 0.99
- Recall (spam): 0.89
- Dataset: 5,500+ labeled SMS messages

## Tech Stack
Python · scikit-learn · Pandas · TF-IDF Vectorizer · Multinomial Naive Bayes

## How it works
1. Raw SMS text vectorized using TF-IDF (stop words removed, max 3000 features)
2. Multinomial Naive Bayes trained on 80% of dataset
3. Tested on 1,115 unseen messages — 98.47% accuracy

## Live prediction example
predict("Win a free iPhone now! Click here")  → spam  
predict("Hey, are we still meeting at 5pm?")  → ham

## Run it yourself
Open spam_email_classifier.ipynb in Google Colab and run all cells.
