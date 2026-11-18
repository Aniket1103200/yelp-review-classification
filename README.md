# Yelp Review Classification (NLP)

Classifies Yelp reviews as **1-star or 5-star** based only on the review text.

> 📚 **Course project:** completed while following the Udemy course *Python for Data Science and Machine Learning Bootcamp* (Pierian Data). The dataset and task come from the course.

## Approach
1. Exploratory analysis of review length and star ratings (Seaborn, Matplotlib)
2. Filtered the data to 1-star and 5-star reviews
3. Converted text to features with **CountVectorizer** (bag of words)
4. Trained a **Multinomial Naive Bayes** classifier
5. Compared it with a **TF-IDF + Naive Bayes** `Pipeline`

## Results (test set: 1,226 reviews)

| Model | Accuracy | Macro F1 |
|---|---|---|
| CountVectorizer + Multinomial Naive Bayes | **0.93** | 0.87 |
| TF-IDF + Multinomial Naive Bayes (Pipeline) | 0.81 | 0.45 |

**Takeaway:** adding TF-IDF made the model worse here. It predicted almost only the majority class (5 stars). The simpler bag-of-words model worked best.

## Tech
Python · pandas · NumPy · scikit-learn · Matplotlib · Seaborn · Jupyter

## Run it
```bash
git clone https://github.com/Aniket1103200/yelp-review-classification.git
cd yelp-review-classification
pip install -r requirements.txt
jupyter notebook yelp_review_classification.ipynb
```
