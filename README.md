# Fake News Prediction

## Overview
This project is a machine learning model that predicts whether a given news article is real or fake. The model is trained using logistic regression on a dataset containing news headlines and authors, with text preprocessing techniques like stemming and stopword removal applied.

## Dataset
The dataset used in this project is loaded from a CSV file (`train.csv`). It includes the following features:
- `author`: The author of the news article.
- `title`: The title of the news article.
- `label`: The target variable (1 for fake news, 0 for real news).



## Preprocessing Steps
1. Fill missing values with an empty string.
2. Create a new `content` column by combining `author` and `title`.
3. Apply text preprocessing:
   - Remove non-alphabetic characters.
   - Convert text to lowercase.
   - Remove stopwords.
   - Apply stemming using the Porter Stemmer.
4. Convert text data into numerical form using `TfidfVectorizer`.

## Model Training
- The dataset is split into training and testing sets (80%-20%).
- Logistic Regression is used for classification.
- The model is trained and evaluated using accuracy scores.

## Accuracy
- **Training Accuracy:** Displayed after fitting the model.
- **Testing Accuracy:** Computed using `accuracy_score`.

## Prediction Example
A sample test case is used to check whether the news is fake or real.

## Running the Project
1. Load the dataset (`train.csv`).
2. Run the Python script to preprocess the data and train the model.
3. Evaluate the model's accuracy.
4. Use the trained model to predict new instances.

## Future Improvements
- Use deep learning models like LSTMs or transformers.
- Add more features for better accuracy.
- Experiment with different ML algorithms.



