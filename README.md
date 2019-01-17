Second project of the Data Analyst Nanodegree by Udacity

The dataset that I wrangled (and analyzed and visualized) was the tweet archive of Twitter user @dog_rates, 
also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. 
These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 
13/10, etc. Why? Because "they're good dogs Brent." WeRateDogs has over 4 million followers and has received international 
media coverage.

The project consisted of 3 steps:

-Data wrangling, which consists of:
  Gathering data
  Assessing data
  Cleaning data

-Storing, analyzing, and visualizing your wrangled data
-Reporting on 1) your data wrangling efforts and 2) your data analyses and visualizations

1. Gathering Data for this Project

- I gathered each of the three pieces of data as described below in a Jupyter Notebook titled wrangle_act.ipynb:

- The WeRateDogs Twitter archive: I Downloaded this file manually

- The tweet image predictions, i.e., what breed of dog (or other object, animal, etc.) is present in each tweet according to 
a neural network. The file (image_predictions.tsv) is hosted on Udacity's servers and was downloaded programmatically 
using the Requests library and the following URL: 
https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv

- Each tweet's retweet count and favorite ("like") count at minimum. Using the tweet IDs in the WeRateDogs Twitter archive, 
I did a query the Twitter API for each tweet's JSON data using Python's Tweepy library and store each tweet's entire set of 
JSON data in a file called tweet_json.txt file. Each tweet's JSON data was written to its own line. Then readed this .txt 
file line by line into a pandas.

2. Assessing Data for this Project
After gathering each of the above pieces of data, I assessed them visually and programmatically for quality and tidiness issues.
Detected and document at least eight (8) quality issues and two (2) tidiness issues in my wrangle_act.ipynb Jupyter Notebook. 

3. Cleaning Data for this Project
I cleaned each of the issues you documented while assessing. This cleaning was performed in wrangle_act.ipynb as well. 
The result was a high quality and tidy master pandas DataFrames.

Storing, Analyzing, and Visualizing Data for this Project
I stored the clean DataFrames in a CSV file with the main one named twitter_archive_master.csv. Analyzed and visualized the 
wrangled data in the wrangle_act.ipynb Jupyter Notebook. 

Reporting for this Project
I Created a written report called wrangle_report that briefly describes your wrangling efforts.

Also, created a written report called act_report that communicates the insights and displays the 
visualization(s) produced from the wrangled data.

