# Tweet classification and sentiment analysis

### 1. Download Tweets using Tweepy library

![alt text](https://user-images.githubusercontent.com/74175283/139527487-62f46004-851e-43ff-93fb-d954f4cdb4cf.png)

I downloaded multiple csv files (for bitcoin, ethereum, cryptocurrencies...) and then merged them all together into crypto_tweet.csv file

### 2. Prepare Tweets for further use

![alt text](https://user-images.githubusercontent.com/74175283/139527599-267b37a3-31c3-4621-bd17-b69e0aebfc71.png)

- remove links, hashtags, mentions
- replace misspelled words with correct words
- remove tweets that contain too little information compared to number of links or hashtags (usually ads or spam)

### 3. Tweet Classification
I noticed that there is a lot of tweets that are just spam, invitations to join projects or new coins. I want to use tweets for sentiment analysis and this kind of tweets don't bring any information about crypto world. That's why I want to mark them as spam and remove from dataset.
I didn't have any training dataset so I manualy labeled 100 tweets, trained model and then used it to classify bigger dataset (400 tweets). Then I checked and fixed missclassified tweets and used this as new training dataset. You can repeat this process multiple times until you get dataset that is big enough.

Then I cleaned it little more, removed stop words, tokenized and lemmatized each tweet.

![alt text](https://user-images.githubusercontent.com/74175283/139527781-4c9b001b-347d-499d-8fd1-c6d9eb9e7d30.png)

Little exploratory data analysis to get feeling about data.

![alt text](https://user-images.githubusercontent.com/74175283/139528414-5c63d82e-4a38-4602-947e-0a9555844d13.png)
