# WWDC21 iPhone13 Analysis
## Project Summary
This analysis looks at Apple’s annual September keynote event where they usually announce new apple products, mainly the new iPhone and compares the keynote data to people’s live reaction data from twitter.
## Data mining 
Apple’s keynote data was gathered through their event’s livestream `closed captions` and was saved into a txt file. For the twitter data a python library called `twint` was utilized to pull the raw data and save it as a csv file.
## Data Pre-processing / Feature Engineering 
The keynote `cc` data was cut to just the part of the event where they start talking about their new iPhone. Twitter data in the other hand needed much more tinkering. First, only tweets tweeted in English language was selected and the raw data was reduced to the most important features or columns that was needed for the analysis and further exploration.

For feature engineering part a little bit of `regular expression` was used to filter out all the URLS, twitter handlers and hashtags from the tweet body. Then `vaderSentiment` was applied to the tweet body creating there more columns that rated each tweet and gave a score representing how `positive`, `neutral` or `negative` the tweets were. After that a function was applied to the tweets that basically grouped and counted positive and negative tweets. 
## Analysis results 
[Click Here!](Analysis_illustration_1.2.pdf)
## Tools/Software:
- Canva
- VS Code
- Python:
  -	pandas
  -	twint
  -	wordcloud
  -	vaderSentiment
