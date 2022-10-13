# WeRateDogs

WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "they're good dogs Brent." WeRateDogs has over 4 million followers and has received international media coverage.

## THE GOAL
The goal is to wrangle WeRateDogs Twitter data to create interesting and trustworthy analyses and visualizations. The Twitter archive is great, but it only contains very basic tweet information. Additional gathering, then assessing and cleaning is required for "Wow!"-worthy analyses and visualization.

## INSTALLATIONS 
`Tweepy` which is an API used to access Twitter conveniently with python

## DATA GATHERING
Three datasetd were used in this project an three different methods were used to access them:
1. **twitter_archive_enhanced.csv**: Directly read fron the csv file
2. **image_predictions.tsv**: Downloaded the file from the URL
3. **tweet_json.txt**: Used the Tweepy library to query additional data via the Twitter API


## Data Accessing

Data accessing involves inspecting your data set for two things:
- Data quality issues
- Lack of tidiness
In the course of accessing the datasets both visually and programmatically I was able to find 9 data quality issues and 2 Tidiness issues


### Quality issues

1. Remove retweets since they are not needed.

2. Update invalid ratings with decimal values.

3. Dropping unnecessary columns in `archive` and `image` dataset.

4. Erroneous datatypes in `archive`, `image` and `tweet` dataset.

5. Replace invalid dog names with NaN..

6. Merge multiple dog states.

7. Change 'None' to NaN(name, doggo, pupper, puppo).

8. Rename column names in `image` table

9. Standarize naming of dog breeds.

### Tidiness issues
1. One variable spans Four columns in `archive` table

2. Combine the three tables(dog type, likes and retweet should be part of the `archive` table)

## Data Cleaning

I cleaned the dataset of the issues above using three steps:
- <b>Define</b> - I defined how you will clean the issue in words
- <b>Code</b> - I converted my definitions into executable code
- <b>Test</b> - I tested my data to ensure my code was implemented correctly

## Data Storing

During the Data Cleaning process, I consolidated the three datasets into one and I stored this dataset as `twitter-master-archive.csv`

## Data Analysis and Visualizations

In this part of the analysis process, I got five insights and and two visualizations from the master dataset.

### Insights
1. The most retweeted tweet was of a Labrador retriever
2. The top rated dog was a Labrador retriever
3. The most popular dog type that was tweeted was the golden retriever
4. Tweet with the highest number of likes
5. Tweet with the lowest number of likes


### Visualization
1. The most retweeted dog state
2. The most popular dog names