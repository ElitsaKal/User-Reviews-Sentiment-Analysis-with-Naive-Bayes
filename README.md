In this project we have text course reviews from students from a data science learning platform. Our aim is to perform sentiment analysis and classify the text reviews as good or bad.
1. Reading the data - We start by reading the file as a pandas data frame and include a few lines to ensure we read the data succesfully by skipping some bad rows.
2. Data types - we check the data types and convert the review column to a numerical type instead of string
3. Exploratory analysis
   a. Histogram - we check the review distribution with a histogram of the review scores.
   ![distribution](https://github.com/ElitsaKal/User-Reviews-Sentiment-Analysis-with-Naive-Bayes/assets/162779608/03bef355-4315-4b23-bcc9-cde1053dad48)

   b. Correlation analysis - we check for correlation between the text review length and the rating
5. Training a Naive Bayes algorithm for review score classification
   a. We start by splitting the data into train and test set
   b. We initialize a vectorizer for the Naive Bayes algorithm
   c. We train a Multinomial Naive Bayes algorithm on the data
   d. We test the classifier
6. Resampling data - We oversample in the minority class to obtain better results
7. Converting the problem to a binary one - we convert the multiclass classification problem to a binary one, by grouping reviews with scores from 1 to 3 as "bad" and scores of 4 and 5 as "good"
8. Resampling data - Again we oversample in the minority class to improve model performance.
9. Model evaluation - we create a classification report showing model performance.
    ![binary_results](https://github.com/ElitsaKal/User-Reviews-Sentiment-Analysis-with-Naive-Bayes/assets/162779608/ee216c4e-d441-4f7b-b6f6-ff2c30d1b471)

10. Model validation - We test the model on new unseen data.
    
![test-set](https://github.com/ElitsaKal/User-Reviews-Sentiment-Analysis-with-Naive-Bayes/assets/162779608/491a0775-4669-4be4-8915-d5fda9b89a24)
