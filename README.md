# Twitter-Sentiment-Analysis
Sentiment Analysis for Racist/Sexist tweets and labelling test dataset after modeling and prediction

Context
The objective of this task is to detect hate speech in tweets. For the sake of simplicity, we say a tweet contains hate speech if it has a racist or sexist sentiment associated with it. So, the task is to classify racist or sexist tweets from other tweets.

Formally, given a training sample of tweets and labels, where label '1' denotes the tweet is racist/sexist and label '0' denotes the tweet is not racist/sexist, your objective is to predict the labels on the test dataset.

Content
Full tweet texts are provided with their labels for training data.
Mentioned users' username is replaced with @user.

Used dataset of Twitter Sentiment Analysis imported from Kaggle with 3 columns intrain dataset id, tweet, label
Test dataset has 2 columns id and tweet

Steps:
1) convert tweets in lowercase
2) with nltk download english stopwords and filter stopwords from tweets
3) with re.sub remove alphanumeric and punctuations
4) now we cau use tokenizer, word2vector, tf-idf for converting words into numeric value for modeling. I am using tokenizer(word frequency in text/document)
5) fit tokenizer for train tweets
6) convert text to sequences
7) pad sequences for uniformity(fixed features/attributes) and build model using embedding, LSTM, Dense, layers
8) compile model with optimizer(Adam)
9) predict test data after modeling
