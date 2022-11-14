# Project: We Rate Dogs Data Wrangling 

## Table of Contents
<ul>
<li><a href="#intro">Introduction</a></li>
<li><a href="#gathering">Data Gathering</a></li>
<li><a href="#assess">Data Assessment</a></li>
<li><a href="#clean">Data Cleaning</a></li>
<li><a href="#conclusions">Conclusion</a></li>    
</ul>

<a id="intro"></a>
## Introduction

This report briefly describes all the wrangling effort carried out on the data from the "WeRateDog" twitter account, a twitter account popular with rating dogs (https://twitter.com/dog_rates). 

<a id='gathering'></a>
## Data Gathering

Data gathering for this project involved gathering data from three different sources requiring different approaches. 
1. The first one is the “twitter_archive_enhanced.csv” file which contains the tweets ids and some other columns. This file was downloaded manually and uploaded on Jupyter notebook environment.


2. The second one is the “image_prediction.tsv” file. This file was downloaded programmatically using the Requests library from a provided URL. This file has image predictions results for the dogs’ breeds obtained using a neural network to make predictions on images from tweets in the twitter archived file.


3. The third dataset is the “tweet_json.txt” file. This file was gathered from twitter’s API using the Tweepy library by querying the API to obtain the retweet count and favorite count. This data was saved as a csv file named ‘Additional data.csv’.


<a id='assess'></a>
## Data Assessment

The three gathered datasets were assessed visually and programmatically.
In this stage. The datasets were assessed for quality and tidiness. Quality issues are related to the content of the data.  These issues are identified by asking questions like;
- Which part of the data is missing?
- Is the data point technically possible?
- Is the data point correct?
- Is it consistent with the rest of the data points?

This is done to check the standards of quality data- criteria of completeness, validity, accuracy, and consistency.
Furthermore, Tidiness issues are related to the structure of the data. To assess the tidy nature of the datasets, questions on whether each variable forms a column, each
observation forms a row and each type of observational unit forms a table were answered.
About nine (9)  issues were identified and documented in the “wrangle_act.ipynb” jupyter notebook.


<a id='clean'></a>
## Data Cleaning

Data cleaning was the most rigorous step in the data wrangling process. The quality and tidiness issues identified in the assessment section were fixed to improve the quality of the “we rate dog” dataset. 

The cleaning followed the process of defining the issues, coding and testing to see if each issue had been resolved.
Most of the cleaning was performed programmatically using functions and some python and pandas inbuilt functions and libraries. However, some were done manually when manually fixing seem faster and more efficient. 


<a id='conclusions'></a>
## Conclusion

The final data cleaning step involved merging all the three cleaned datasets as a single csv file to be used for further analysis. This dataset was saved as “twitter_archive_master.csv’ . This file can be improved upon depending on the end goal of any future analysis or usage.
