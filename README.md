---

# IMDB Movie Sentiment Analysis

## Project Overview
This project focuses on performing **sentiment analysis** on the IMDB movie reviews dataset, consisting of 50,000 reviews. The primary goal was to build a robust classification model that can accurately distinguish between positive and negative reviews.

## Step 1: Data Cleaning and Preprocessing
The first crucial step in any **Natural Language Processing (NLP)** task is to clean and preprocess the data.

- **Regular Expressions**: Utilized to remove unwanted characters, patterns, and noise from the text data, ensuring a cleaner input for analysis.
- **Vectorization**: Converted textual data into numeric form through vectorization. This allows machine learning algorithms to process and understand the textual information effectively.

## Step 2: Building the Baseline Classifier
To start, we constructed a baseline model using **Logistic Regression** due to its interpretability and efficiency with sparse datasets.

- **Logistic Regression**:
  - **Interpretability**: Easy to understand and interpret results.
  - **Performance**: Works well with sparse datasets like the one used in this project.
  - **Speed**: Quick learning process, ideal for initial model testing.
- **Hyperparameter Tuning**: Focused on adjusting the **C** parameter to fine-tune regularization, balancing bias and variance.

## Step 3: Text Processing for Improved Accuracy
To enhance model accuracy, several text processing techniques were applied:

- **Stop Words Removal**: Removed common, insignificant words to reduce noise and improve the focus on meaningful content.
- **Normalization**: Standardized text data to ensure consistency.
- **Stemming and Lemmatization**: Reduced words to their base forms, helping to treat variations of the same word as equivalent.
- **N-grams**: Captured sequences of words (unigrams, bigrams, trigrams) to consider context and improve the model's understanding.
- **Word Count and TF-IDF Representations**: Implemented **TF-IDF** (Term Frequency-Inverse Document Frequency) to weigh words by importance, enhancing the model's ability to prioritize significant terms.

## Step 4: Advanced Model Selection
To further improve the model’s accuracy, a more sophisticated algorithm was tested:

- **Support Vector Machine (SVM)**: Utilized a **Linear SVM** classifier, known for its effectiveness with high-dimensional and sparse datasets. By experimenting with different **n-gram ranges** (1 to 3), we achieved significant accuracy improvements.

## Final Model
The final model was built by combining the optimal text processing techniques with the **Linear SVM** classifier.

- **Best Results**: Removing specific stop words, using an n-gram range of 1 to 3, and applying a Linear SVM provided the most accurate results in classifying sentiment.
- **Achieved Accuracy**: Surpassed the **90% accuracy** mark, demonstrating the effectiveness of the chosen techniques and algorithms.

## Summary
This project explored various techniques for text transformation and model selection to maximize the accuracy of an NLP model. The results showed that a combination of careful preprocessing, feature engineering, and algorithm selection could yield highly accurate and reliable sentiment analysis models. Continuous experimentation with different combinations of these techniques is crucial for achieving the best results in similar tasks.

---

