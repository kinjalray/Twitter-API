# Twitter-API
Wrangle @WeRateDogs tweets data


I broke down my data wrangling in 3 steps: Gathering, Assessing, and Cleaning data. 

## Gathering
I gathered data from three different sources:
1. csv file source for ‘twitter-archived-enhanced.csv.’ This data consists of tweet data for the We Rate Dogs twitter account, with variables including: replies, retweets, dog stages, text in the tweet, and tweet sources. 
2. I programmatically pulled from an URL. This data set consists of image predictions corresponding to the tweets in the archive dataset. For example, both the archive and the image predictions data has the “tweet_id” column. For each image associated with a tweet, the image predictions file share predictions for what type of dog breed the image shows. 
3. Lastly, the third dataset was pulled from the twitter API. This data consists of the tweet id and the number of retweets and favorites. 

## Assessing
In this phase of my wrangling process, I broke down my assessment of the data in 2 categories: data quality and data tidiness.

I noticed 8 outstanding data quality issues and 2 data tidiness issues. The 8 data quality issues are related to the archive dataset, which had the “dirtiest” data. I fixed columns up by changing data types and assigning the correct dog stage based on the contents of the corresponding tweets. 

In terms of tidiness, all three datasets belong in one comprehensive table as they all contain information about tweets, a single observational variable.
To see full documentation of the data quality issues, see the WeRateDogs.ipynb file. 

## Cleaning
Lastly, after documenting the necessary changes required to improve the data quality for analysis, I programmatically addressed the data issues by systematically tackling one task at a time.  
