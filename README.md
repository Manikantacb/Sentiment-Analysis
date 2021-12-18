# Sentiment-Analysis

1. Github repo created.
2. Data exported from Telegram https://t.me/CryptoComOfficial from May 1 to
and including May 15, 2021.
Data can be found in results.json file
3. Data is preprocessed to remove non-English messages and filtered to include only messages either having “SHIB” or “DOGE.”
4. Sentiment of each message is computed and displayed on the analysis column.
5. Using cufflinks and plotly the visualizations are displayed.

# Summary

1. Import libraries
2. Read Data from json file
3. Data Preprocessing.
The Preprocessing steps involve the following:
a. Cleaning the text: Removing unwanted characters.
b. Tokenization: Tokenization is done using nltk tokenizer
b. Enrichment-POS tagging: Parts of Speech (POS) tagging is a process of converting each token into a tuple having the form (word, tag). POS tagging essential to preserve the context of the word and is essential for Lemmatization.
c. Stopwords removal: These words are removed as they do not give any useful information.
d. Lemmatization: Obtaining the stem words.

4.Sentiment Analysis using TextBlob
TextBlob is a python library used for processing textual data. It is used for sentiment analysis, part-of-speech tagging.

The two measures that are used to analyze the sentiment are:

Polarity – talks about how positive or negative the opinion is
Subjectivity – talks about how subjective the opinion is
TextBlob(text).sentiment gives us the Polarity, Subjectivity values.
Polarity ranges from -1 to 1 (1 is more positive, 0 is neutral, -1 is more negative)
Subjectivity ranges from 0 to 1(0 being very objective and 1 being very subjective)

Using the polarity and the analysis method we find out the sentiment for each text.

From my analysis I found out that out of all messages 393 of them have the word 'SHIB' or 'DOGE.'
After data preprocessing and sentiment analysis I found out that 66.2% of the messages are 'Neutral', 22.4% of the messages are 'Positive' and 11.5% of the messages are 'Negative'.

The number of messages per day is plotted using plotly and cufflinks.

