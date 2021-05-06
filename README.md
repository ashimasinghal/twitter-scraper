# twitter-scraper
# scweet
### Offical repo- https://github.com/Altimis/Scweet
.
### wiki- 
In the last days, Twitter banned almost every twitter scrapers. This repository represent an alternative legal tool (depending on how many seconds we wait between each scrolling) to scrap tweets between two given dates (start_date and max_date), for a given language and list of words or account name, and saves a csv file containing scraped data 

[UserScreenName, UserName, Timestamp, Text, Embedded_text, Emojis, Comments, Likes, Retweets, Image link, Tweet URL]

Tweets :
The CSV file contains the following features (for each tweet) :

'UserScreenName' :
'UserName' : UserName
'Timestamp' : timestamp of the tweet
'Text' : tweet text
'Embedded_text' : embedded text written above the tweet. It could be an image, video or even another tweet if the tweet in question is a reply.
'Emojis' : emojis existing in tweet
'Comments' : number of comments
'Likes' : number of likes
'Retweets' : number of retweets
'Image link' : Link of the image in the tweet
'Tweet URL' : Tweet URL.

# important columns: 
'hashtags' : hashtags appearing in each tweet

'preprocessed words' : words deeply pre processed and tokenized

*can further increase the functionality by accessing Following / Followers, reposts, user information *


## The folder contains 4 subfolders:
# FOLDER 1 - Code:
scweet: Actual notebook containing the code for the scraper
num2words: code used to convert numerics to word numerals
preprocessing: code used to clean the text. I have cleaned in two formats-
1. created column in df with cleaned words, applied lemmatization, removed stopwords, stemming, etc.
output file- df_final.csv
2. removed punctuations, links, hashtags, emojis, etc in sentence format
output file- processed sentences.txt

# FOLDER 2 - output:
1. preprocessed_tweets.csv- real data with column processed_words containing preprocessed words, can be used directly for tasks like NER, SA, etc
2. processed sentences.txt - about 10k cleaned sentences
3. frequent_words.png - image generated plotting most frequent words appeared in the lot

# FOLDER 3 - raw:
1. df_final.csv - file with all the original scraped tweets.
2. raw sentences.txt - raw sentences
