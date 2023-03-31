# wrangle-WeRateDogs-data
Wrangling and analyzing the WeRatesDogs Twitter data

This was the 2nd project I carried out as part of my Udacity Data Analyst Nanodegree program. The project was carried out in 3 major phases; Data gathering, Data Assessment/Cleaning, and Data Visualization. 

The data gathering step involved gathering, loading and combining three different pieces of data. The first data containing the WeRateDogs Twitter archive data was provided by Udacity and stored in a csv titled, twitter_archive_enhanced.csv. It consist of 17 distinct columns and a total of 2,356 data entries. This file was downloaded manually via the following [link](https://d17h27t6h515a5.cloudfront.net/topher/2017/August/59a4e958_twitter-archive-enhanced/twitter-archive-enhanced.csv). 

The second dataset contained predictions of tweet images up until August 1st 2017 recorded under the 'expanded_urls' column in the twitter_archive_enhanced.csv file. The image predictions were made using a neural network and the data was hosted on Udacity's servers. I used the Requests library to programmatically download the data via the [URL](https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv) and stored it as image_predictions.tsv. This file contains 12 columns and 2,075 data entries. 

Finally, I made use of the Tweepy library to query additional data including the 'retweet_count' and 'favorite_count' for the WeRates Twitter archive data and stored this information in a json file named tweet_json.txt.

After data gathering, I went on assess the data both visually and programmatically. From this step, I was able to identify and clean nine(9) data quality issues and two(2) tidiness issues, while adhering to the rules of [tidy data](https://cran.r-project.org/web/packages/tidyr/vignettes/tidy-data.html). The result of the cleaned data is a high-quality and tidy pandas dataframe stored in a CSV file. 

Finally, for data visualization, some exploratory data analysis was further carried out on the cleaned data. At the end of the project, I was able to wrangle, analyze and visualize the cleaned data, while gaining some meaningful insights.
