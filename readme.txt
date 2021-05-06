The folder contains 4 subfolders:
FOLDER 1 - Code:
scweet: Actual notebook containing the code for the scraper
num2words: code used to convert numerics to word numerals
preprocessing: code used to clean the text. I have cleaned in two formats-
1. created column in df with cleaned words, applied lemmatization, removed stopwords, stemming, etc.
output file- df_final.csv
2. removed punctuations, links, hashtags, emojis, etc in sentence format
output file- processed sentences.txt

FOLDER 2 - output:
1. preprocessed_tweets.csv- real data with column processed_words containing preprocessed words, can be used directly for tasks like NER, SA, etc
2. processed sentences.txt - about 10k cleaned sentences
3. frequent_words.png - image generated plotting most frequent words appeared in the lot

FOLDER 3 - raw:
1. df_final.csv - file with all the original scraped tweets.
2. raw sentences.txt - raw sentences
