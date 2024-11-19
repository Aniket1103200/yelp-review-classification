# yelp-review-classification
A project focusing on text classification using Natural Language Processing (NLP) techniques. The goal is to classify Yelp reviews into 1-star or 5-star categories based on review content. The project implements data preprocessing, feature engineering, and machine learning pipeline methods for efficient and accurate classification.

# Yelp Review Classification

Welcome to the **Yelp Review Classification Project**! 🚀

## Overview
This project is designed to classify Yelp reviews into **1-star** or **5-star** categories based on the textual content of the reviews. Using the **Yelp Review Data Set** from Kaggle, we explore the power of NLP and machine learning to solve this classification problem.

## Problem Statement
Each observation in the dataset represents a review of a business. Our goal is to classify these reviews into binary categories (1-star or 5-star) using their textual content. This involves:
- Text preprocessing and tokenization.
- Feature extraction using vectorization techniques.
- Implementing a classification pipeline.

## Features Used
- **Text Content:** The main review content.
- **Stars:** Target column representing the rating (1 or 5 stars).

## Methodology
1. **Data Cleaning & Preprocessing:**
   - Handled missing values and irrelevant data.
   - Processed text data (removing stopwords, lowercasing, etc.).

2. **Feature Engineering:**
   - Implemented `CountVectorizer` and `TF-IDF` for text vectorization.

3. **Pipeline Creation:**
   - Combined vectorization with a classification model (`Naive Bayes`).

4. **Evaluation Metrics:**
   - Accuracy
   - Precision
   - Recall

5. **Insights:**
   - Explored the relationship between review content and star ratings.
   - Visualized word usage frequency and sparsity.

## Results
Achieved high classification accuracy using a combination of `TF-IDF` and `Multinomial Naive Bayes`. Detailed evaluation metrics and plots are provided in the Jupyter Notebook.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Aniket1103200/yelp-review-classification.git
