
## Dataset

The dataset that I will be wrangling, analyzing and visualizing is the tweet archive of Twitter user @dog_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "they're good dogs Brent." WeRateDogs has over 4 million followers and has received international media coverage.

WeRateDogs downloaded their Twitter archive and sent it to Udacity via email exclusively for me to use in this project as a student at Udacity. This archive contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ of their tweets as they stood on August 1, 2017.

## Process

Firstly, i imported the libraries i may need in the course of my wrangling process. The library included pandas, numpy, matplotlib, seaborn, request, tweepy, json etc.
There are three files I worked with. i. Twitter-archive-enhanced.csv (Contains dog ratings) ii. image_predictions.tsv (Predicts if tweets really contained dog images) iii. tweet_json.txt (Contains the retweet counts and users tweet favorite counts) I then read the "twitter-archive-enhanced.csv" and represented it as df1. This file contained tweeter users tweets for a dog rating twitter account, We Rate Dogs. The table contained the tweet id, timestamp, text, rating numerator, rating denominator, dog names, dog type (doggo, puppo, pupper, floofer) among others. I displayed the table for visual assessment and noted down some issues. Then I used the "requests library" to download the tweet image prediction (image_predictions.tsv) from the image prediction url. This I used to predict if the images in df1 (tweeter archive) are indeed dogs. I then read the file and displayed it for a quick visual assessment. I also noted down some quick issues I identified, such as wrong images. After, I used the "Tweepy library" to query additional data (retweet counts and favorite counts) via the Twitter API (tweet_json.txt). I also read and displayed it for a quick visual assessment. I assessed and analysed the tables using both visual and programmatic assessment and analysis, identified and listed out 8 quality issues as required for the project and 2 tidiness issues, and cleaned the data. In cleaning, I first define what to do, write the codes and test it afterwards. In the process of cleaning, I copied the files and used the copy for the cleaning process. This is to avoid losing data in case of permanent changes that are irreversible. I cleaned the data and stored it in a CSV file named "twitter_archive_master.csv".

## Findings

Programmatic assessment was also conducted to get some insights, and it was found out that most users rated their dogs at 12/10. Assessment also revealed that the tweet that majority users chose as their favorite was that of a picture of a puppo dog with tweet id 822872901745569793. This was found out by using 'describe' to check for the max value in the "favorite_count" column, which value is then traced to check for the tweet and dog name. Also, the tweet that majority of users retweeted was that of a picture of a doggo dog with tweet id 744234799360020481. This was found out by using 'describe' to check for the max value in the "retweet_count" column, which value is then traced to check for the tweet and dog name. The visualization displays the number of dogs that were identified as doggo by users who tweeted, compared to those who are not or who are were not identified at all. In the doggo column, 87 dogs were identified as doggo while 2079 other dogs were either listed as other dog types or not listed at all. Not listing the dog type might have been due to many things including errors and oversight from users. It could also be deliberate. I however made sure I cleaned the data to remove all invalid tweets. 

## Insights

1. Most dogs are rated 12
2. Most users choosed tweet with id 822872901745569793 as their favorite with is a puppo dog
3. Tweet with id 744234799360020481 is the most retweeted tweet which is a doggo dog

