# Twitter Sentiment Analysis (NLP)

## Project Overview
This project is a Natural Language Processing (NLP) model built to analyze the sentiment of text data. It is trained on a downsampled, perfectly balanced subset (100,000 tweets) of the Sentiment140 dataset to classify text as either Positive or Negative.

## Technical Stack
* **Framework:** Scikit-Learn, Pandas
* **Language:** Python
* **Environment:** Google Colab
* **Dataset:** Kazanova/Sentiment140 (via Kaggle API)

## Pipeline Architecture
1. **Text Preprocessing:** Custom regex cleaning to strip URLs, @mentions, hashtags, and punctuation, followed by lowercase normalization.
2. **Vectorization:** TF-IDF (Term Frequency-Inverse Document Frequency) limited to the top 10,000 most common features.
3. **Classification:** Logistic Regression model (max_iter=1000).

## Performance
* **Testing Split:** 20%
* **Final Accuracy:** ~78.30%
