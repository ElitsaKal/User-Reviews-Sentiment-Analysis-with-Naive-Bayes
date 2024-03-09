In this project we have text course reviews from students from a data science learning platform. Our aim is to perform sentiment analysis and classify the text reviews as good or bad.
1. Reading the data - We start by reading the file as a pandas data frame and include a few lines to ensure we read the data succesfully by skipping some bad rows.
2. Data types - we check the data types and convert the review column to a numerical type instead of string
3. Exploratory analysis
   a. Histogram - we check the review distribution with a histogram of the review scores.
   b. Correlation analysis - we check for correlation between the text review length and the rating
4. Training a Naive Bayes algorithm for review score classification
   a. We start by splitting the data into train and test set
   b. We initialize a vectorizer for the Naive Bayes algorithm
   c. We train a Multinomial Naive Bayes algorithm on the data
   d. We test the classifier
5. Resampling data - We oversample in the minority class to obtain better results
6. Converting the problem to a binary one - we convert the multiclass classification problem to a binary one, by grouping reviews with scores from 1 to 3 as "bad" and scores of 4 and 5 as "good"
7. Resampling data - Again we oversample in the minority class to improve model performance.
8. Model evaluation - we create a classification report showing model performance.
9. Model validation - We test the model on new unseen data.
