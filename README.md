# AssignmentSMWA2020Group4

The files are grouped into several parts.
1. General setup
2. User Reviews
3. Critics Reviews
4. Twitter
5. Model
6. Scrape Data
7. data (folder)
8. output (folder)

## General setup
General setup consists of:
1. General_0_Set_Up  
  1.1 Sets the working directory  
  1.2 Sets global variables
2. General_1_Preprocessing  
  2.1 Defines some general text processing functions that are further used in user reviews, critic reviews and twitter documents  

These documents should be ran before any of the other files.

## User Reviews
User Reviews consists of:
1. User_Reviews_0_Set_Up  
  1.1. Reads in the data  
2. User_Reviews_1_Preprocessing  
  2.1 Cleans the text data 
3. User_Reviews_2_Sentiment_Analysis  
  3.1 Performs dictionary based sentiment analysis en aggregates the result into a basetable later used in the model  

These documents should be ran in order.
  
## Critic Reviews
Critic Reviews consists of:
1. Critics_Reviews_0_Set_Up  
  1.1. Reads in the data  
2. Critics_Reviews_1_Preprocessing  
  2.1 Cleans the text data 
3. Critics_Reviews_2_Sentiment_Analysis  
  3.1 Performs dictionary based sentiment analysis en aggregates the result into a basetable later used in the model
  
These documents should be ran in order.
  
## Twitter
Twitter consists of:
1. Twitter_0_Set_Up  
  1.1. Reads in the data  
2. Twitter_1_Preprocessing  
  2.1 Cleans the text data 
3. Twitter_2_1_Sentiment_Analysis  
  3.1 Performs dictionary based sentiment analysis en aggregates the result into a basetable later used in the model  
4. Twitter_2_2_Extra_Features  
  4.1 Extracts follower count of all movie twitter pages  
  4.2 Calculates ratio of owned media posts that contain a photo to measure variety  
5. Twitter_2_3_LSA  
  5.1 Performs LSA on earned media posts  
6. Twitter_2_4_Stars  
  6.1 Searches stars names extracted from imdb on twitter and attempts to find matching twitter profiles  
  6.2 Extracts follower counts of matched profiles and aggregate per movie  
7. Twitter_3_1_Boxplots_Sentiment_before_cleaning
8. Twitter_3_2_Boxplots_Sentiment_after_cleaning
9. Twitter_4_Bloodshot_time_evolution
10. Twitter_5_Bloodshot_Contribution_to_Sentiment
11. Twitter_6_Bloodshot_popular_bigrams

These documents should be ran in order.

## Model
Model consists of:
1. Basetable_Creation  
  1.1. Aggregates all basetables created in previous document to be used for the modelling  
2. Modeling  
  2.1 Creates random forest model and performs some analysis
  
## Scrape Data
Scrape_Data consists of:
1. Scrape_Data.R
  1.1 Scrapes the movie's twitter profile tweets and tweets from each movie's respective hashtag  
  1.2. Stored in data/twitter  
2. Imdb_Scrape.ipynb  
  2.1 Python notebook file that scrapes the imdb pages of all the movies  
  2.2 Follows links to user and critic reviews  
  2.3 Scrapes user and critic reviews  
  2.4 Stored in data/imdb
3. The_Numbers_Scrape.ipynb  
  3.1 Python notebook file that scrapes the weekend box office sales  
  3.2 Stored in data/box_office
  
## data
Folder of csv's that are used in the R files

## output
Folder of output from graphs
