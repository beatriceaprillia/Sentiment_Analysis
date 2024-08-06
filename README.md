# Sentiment_Analysis
The aim of this project is to perform sentiment analysis on a dataset of Indonesian reviews. The project involves preprocessing the text data, building a classification model, and visualizing the results to understand the sentiment of the reviews.

## Dataset:
data_real.csv: Contains original review data with a 'Rating' column indicating the sentiment (1 or 2 for negative, and 3, 4, or 5 for positive).

## Steps Involved:
1. Data Loading and Preprocessing:
   - Read the dataset.
   - Handle missing values by filling them with a placeholder text.
   - Perform text preprocessing such as case folding (lowercasing the text), removing stop words, and stemming (reducing words to their root form).
2. Text Vectorization:
   - Convert the cleaned text data into a numerical format using CountVectorizer to create a term-document matrix.
   - Calculate term frequencies for the entire dataset and individual reviews.
3. Labeling the Data:
   - Create a binary label (0 for negative and 1 for positive) based on the rating provided in the dataset.
4. Model Building and Evaluation:
   - Split the data into training and test sets.
   - Train a Gaussian Naive Bayes model on the training data.
   - Evaluate the model using a confusion matrix and classification report.
   - Visualize the model's performance using ROC curve.
5. Visualization:
   - Plot the confusion matrix to show the number of correct and incorrect predictions.
   - Display the ROC curve to evaluate the model's performance in distinguishing between the positive and negative classes.

## Tools and Libraries:
1. Pandas: For data manipulation and analysis.
2. Matplotlib & Seaborn: For data visualization.
3. Sastrawi: For Indonesian text preprocessing (stop words removal and stemming).
4. Scikit-learn: For machine learning algorithms and evaluation metrics.

This project provides a comprehensive pipeline for sentiment analysis on Indonesian reviews, from text preprocessing to model building and evaluation. The ROC curve visualization helps in understanding the model's performance in distinguishing between positive and negative sentiments.
