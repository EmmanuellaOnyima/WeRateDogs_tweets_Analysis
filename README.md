# WeRateDogs Tweet data Exploration

## By Emmanuella Onyima

## Dataset
The dataset consists of the following dataframes required for the analysis:

>- **the twitter archive data**. It can be gotten [here]('twitter-archive-enhanced (1).csv'). this contains basic tweet data for all 5000+ of their tweets, but not everything. It has been filtered for tweets with ratings only, resulting to 2356 tweets.

>- **the image prediction data** ('image-predictions.tsv') which will be downloaded programmatically from the [link](https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv'). This classifies what breed of dog that is present in each tweet according to the previously created neural network.

>- **Additional data via twitter API**: there are data omissions (retweet count and favorite count) found in the twitter archive data, which will be gotten by querying the twitter API. Using the tweet IDs in the WeRateDogs Twitter archive, the Twitter API for each tweet's JSON data will be queried using Python's Tweepy library and each tweet's entire set of JSON data will be stored in a file called tweet_json.txt file. Each tweet's JSON data would be written to its own line. Then the .txt file read line by line into a pandas DataFrame with tweet ID, retweet count, and favorite count.

## Summary of Findings
In the exploration , I discvered the following insights:
> 1. The highest tweets occured between the November 2015 to January 2016 and decreased across 2017.

> 2. The highest favorite tweets occured on the 21st of january 2017 (2017-01-21 18:26:02+00:00).

>3. The top three predicted dogs with the highest favorite counts include:

>- Lakeland_terrier
>- Labrador_retriever
>- English_springer

>4. Puppo is the dog stage with the highest favorite count.

>5. There is a positive correlation between the favorite_count and retweet count, meaning that there is an increase in the favorite_count corresponding to an increase in the retweet count.

>6. There is a positive correlation between the timestamp and the favorite_count which means that there was an increase in favorite count over time




