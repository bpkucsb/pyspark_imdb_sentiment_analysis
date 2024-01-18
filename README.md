# pyspark_imdb_sentiment_analysis
Supervised learning using imdb movie reviews to predict positive and negative sentiment

The dataset was taken from the following academic site (Maas, Andrew L.  and  Daly, Raymond E.  and  Pham, Peter T.  and  Huang, Dan  and  Ng, Andrew Y.  and  Potts, Christopher, Learning Word Vectors for Sentiment Analysis, June 2011):

https://ai.stanford.edu/~amaas/data/sentiment/

Here I do a simple word extraction, removing stop words and doing term frequency inverse document frequency transformations in a PySpark pipeline before having a logistic regression predict sentiment analysis based off of the text data.

This is a bare bones analysis in PySpark and future iterations should include n-gram analysis as well as lemmatization and additional NLP cleanups of the reviews to improve model performance.

The final logistic regression model has a ROC AUC of 0.83, which will be improved in future iterations.
