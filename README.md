This project performs sentiment analysis on IMDB movie reviews using Natural Language Processing (NLP) and machine learning. It classifies reviews as either positive or negative using a Naive Bayes classifier.

OWorkflow Summary
1. Data Loading
The dataset IMDB Dataset.csv is loaded, which contains two columns:

review: the text of the review

sentiment: the label (positive or negative)

2. Text Preprocessing
Each review goes through the following steps:

Convert text to lowercase

Remove HTML tags and non-alphabetic characters

Tokenize words

Remove stopwords

Apply lemmatization to normalize words

3. Feature Extraction
Text is converted into numeric format using TF-IDF Vectorizer with a maximum of 5000 features.

4. Model Training
The data is split into training and testing sets.
A Multinomial Naive Bayes classifier is trained on the TF-IDF features.

5. Model Evaluation
The model's performance is evaluated using the classification report (Precision, Recall, F1-Score).

6. User Input Prediction
The user can enter a custom review, and the model will predict whether it is Positive or Negative sentiment.

Example
Input:
The movie was absolutely wonderful!

Output:
Predicted Sentiment: Positive 

Requirements
pandas

numpy

nltk

scikit-learn

Install missing libraries using pip install.
