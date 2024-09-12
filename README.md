# Sentiment Analysis on Review Data
# Overview
This project performs sentiment analysis on review data using text classification techniques. The primary goal is to classify reviews into 'good' or 'bad' categories based on their ratings. The project involves data preprocessing, model training, evaluation, and visualization. The final model is tested on a cleaned dataset to ensure its effectiveness.

# Dataset
File: usercourses.csv
Description: Contains reviews with ratings and comments.
Columns:
review_comment: The text of the review.
review_rating: The rating given in the review.
# Steps and Methodology
# 1. Data Cleaning and Preprocessing
Handle Missing Values: Removed rows with missing values in review_comment or review_rating.
Convert Ratings: Converted review_rating to numeric, handling any conversion issues.
Text Cleaning: Applied a function to clean and normalize text data by removing punctuation and converting to lowercase.
# 2. Binary Classification
Convert Ratings to Binary: Transformed ratings into binary labels ('good' for ratings >= 4 and 'bad' otherwise).
Class Imbalance Handling: Oversampled the minority class to balance the dataset.
Feature Extraction: Used TF-IDF vectorization to convert text into numerical features.
Model Training: Trained a Naive Bayes classifier using the upsampled dataset.
# 3. Evaluation
Confusion Matrix: Visualized the performance using a confusion matrix plotted as a heatmap.
Classification Report: Generated a detailed classification report showing precision, recall, and F1-score for each class.
Test Set Evaluation: Applied the trained model to a cleaned test set to assess its performance on unseen data.
# Requirements
• pandas
• numpy
• scikit-learn
• matplotlib
• seaborn
• re
# How to Use
Clone the repository:
git clone https://github.com/AbhishekOjha-01/MachineLearningCA2Assignment.git
Navigate to the project directory:
cd MachineLearnnigCA2
Install the required packages:
pip install -r requirements.txt
Run the Jupyter notebook or Python scripts to perform sentiment analysis.
# License
This project is licensed under the MIT License - see the LICENSE file for details.

# Acknowledgments
Thanks to ChatGPT for assistance with code snippets and explanations.
