1. Spam Email Classifier

A machine learning model that classifies SMS messages as spam or legitimate (ham).

## Results
- Accuracy: 98.47%
- Precision (spam): 0.99
- Recall (spam): 0.89
- Dataset: 5,500+ labeled SMS messages

2. Tech Stack
Python · scikit-learn · Pandas · TF-IDF Vectorizer · Multinomial Naive Bayes

3. How it works
1. Raw SMS text is vectorized using TF-IDF (removes stop words, max 3000 features)
2. Multinomial Naive Bayes model trained on 80% of the dataset
3. Tested on 1,115 unseen messages — achieves 98.47% accuracy

4. Live prediction example
```python
predict("Win a free iPhone now! Click here")  # → spam
predict("Hey, are we still meeting at 5pm?")  # → ham
```

5. Run it yourself
Open `spam_email_classifier.ipynb` in Google Colab and run all cells.
