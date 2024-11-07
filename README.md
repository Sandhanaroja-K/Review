# Capstone Project - E-commerce Customer 
# Review Analysis

 
# Table of Contents
1. Problem Statement
2. Project Objective
3. Data Description
4. Data Pre-processing Steps and Inspiration
5. Exploratory Data Analysis (EDA)
6. Sentiment Analysis
7. Insights and Trends
8. Conclusion
9. References
    
## 1. Problem Statement
An e-commerce company has tasked me with analyzing customer reviews for various products. The 
goal is to classify products based on customer reviews and extract useful insights about product 
quality.

## 2. Project Objective
The primary objective is to:
1. Identify trends and patterns in the reviews.
2. Classify each review based on the sentiment associated with it using Naive Bayes and VADER 
models.

## 3. Data Description
The dataset `Reviews.csv` consists of 60,145 rows and 10 columns:
- Id: Record ID
- ProductId: Product ID
- UserId: User ID who posted the review
- ProfileName: Profile name of the User
- HelpfulnessNumerator: Numerator of the helpfulness of the review
- HelpfulnessDenominator: Denominator of the helpfulness of the review
- Score: Product Rating (1-5)
- Time: Review time in timestamp
- Summary: Summary of the review
- Text: Actual text of the review
- 
## 4. Data Pre-processing Steps and Inspiration
Initial Data Exploration
- Load the dataset and examine its structure.
- Check for missing values, duplicates, and outliers.
- Convert timestamps to readable date formats.
Data Cleaning
- Handle Missing Values: Impute or remove missing values.
- Remove Duplicates: Ensure no duplicate entries.
- Correct Data Types: Convert columns to appropriate data types.
  
## 5. Exploratory Data Analysis (EDA)
Descriptive Statistics
- Summary statistics for numerical columns.
- Distribution of product ratings.
- Frequency of reviews over time.
Helpfulness Analysis
- Calculate the helpfulness ratio (HelpfulnessNumerator / HelpfulnessDenominator).
- Analyze the distribution of helpfulness scores.
Visualization
- Plot the distribution of product ratings.
- Visualize the number of reviews per product.
- Analyze the helpfulness of reviews over time.
- Create word clouds to visualize the most frequent words in positive and negative reviews.
  
## 6. Sentiment Analysis
Text Pre-processing
- Tokenization: Split text into words.
- Stop Word Removal: Remove common words that do not contribute to sentiment.
- Stemming/Lemmatization: Reduce words to their base or root form.
Sentiment Classification
Using Naive Bayes
1. Labeling: Label reviews as positive (Score > 3), neutral (Score = 3), or negative (Score < 3).
2. Feature Extraction: Convert text data to numerical data using techniques like TF-IDF.
3. Model Training: Train a Naive Bayes classifier on the labeled data.
4. Evaluation: Evaluate the model's performance using metrics like accuracy, precision, recall, and F1-
score.
Using VADER
1. Text Pre-processing: Preprocess text data.
2. Sentiment Scoring: Use VADER to score the sentiment of each review.
3. Classification: Classify reviews based on VADER sentiment scores.
   
## 7. Insights and Trends
Trends in Reviews
- Identified common themes in positive and negative reviews using topic modeling (e.g., LDA).
- Analyzed the relationship between review length and rating.
- Identified peak times for positive or negative reviews.
Product Quality Insights
- Classified products based on aggregated sentiment scores from both Naive Bayes and VADER.
- Identified products with consistently high or low ratings.
- Analyzed the correlation between helpfulness scores and review sentiment.
  
## 8. Conclusion
The analysis provides valuable insights into customer sentiment and product quality. By classifying 
reviews and identifying trends using both Naive Bayes and VADER models, the e-commerce company 
can:
- Improve product offerings based on customer feedback.
- Address common issues highlighted in negative reviews.
- Enhance marketing strategies by focusing on positively reviewed products.
  
## 9. References
- "Sentiment Analysis of Customer Reviews using VADER and Machine Learning" by J. Singh et 
al. (2020)
- "Visualizing Customer Sentiment using Word Clouds and VADER" by M. Kumar et al. (2019)
