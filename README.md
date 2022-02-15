# Yelp Capstone Project
This is my capstone project for my Bachelor of Applied Science in Data Analytics. The data set used is provided from Yelp through their open dataset initiative. It can be downloaded from their website or from Kaggle. This dataset consists of over 10GB's of JSON and includes over 8 million reviews, 160 thousand business, and 8 metropolitan areas. The dataset also recorded information about business operating hours, parking availability, and if free WiFi was provided. My variable of interest is whether the business was listed as opened or closed. 

# Purpose
This project’s purpose is to find what common attributes help predict whether a business is open or not. Based on that, can I accurately predict if a business has stayed open or permanently closed. There are a multitude of reasons for why a business decides to close and many of those reasons cannot be provided just through the Yelp dataset. A question we might ask is if this is even needed if we can assume businesses with low stars are more likely to go out of business. Is it possible to make a general prediction? Another question that needs to be answered is if the same could be said about location, can we also assume the success of a business based on where they do business? These questions not only ask us to predict what affects the outcome but also why it affects their success or failure as a business. 

# Customer
The potential customer that would be most assisted by my solution would be business owners, real estate investors, landlords, and potential entrepreneurs. Business owners might want to find a new place to move to or where to build their next branch. Real estate investors who not only want the land to be valuable but also that the business on top of it increases the valuation. Landlords who want to make sure that the most successful business not only rents from them but also can not fall behind on rent or go in debt. Finally, entrepreneurs who are looking into starting a small business and want to know where the best location is for certain industries. 

# Tools Used
The tools primarily used in my project are python and MongoDB. I used python for data analysis and machine learning while I created a MongoDB database to store my data. In addition, software and packages used consisted of Docker, Jupyter Notebook, pandas, scikit learn, and matplotlib.

# Data Preprocessing 
For data cleaning, I used dummy variables for my categorical data and standardized the text by removing empty spaces and unneeded punctuation. I then made the data case insensitive by converting it all to lowercase. The reason for this was that many city names were not formatted correctly and it considered two of the same places as different cities. I have also removed any businesses that had missing data.

# Machine Learning
I primarily used supervised learning classification models from the python library scikit-learn. The 4 I have decided to evaluate are KNN, Naive Bayes, Decision Trees, and Random Forest. To create an accurate model for each algorithm, I have also elected to use k-Fold Cross Validation instead of creating a static test and training data set. I found that the model that could accurately predict whether a business was open or closed the most was Random Forest. The next best model was KNN, followed by Decision Trees and then Naive Bayes.

Random Forest was the best model out of the 4 tested with an average accuracy score of 79.85%.
Some possible improvements to the model would probably consist of  dimensionality reduction, feature scaling, and hyperparameter tuning.

# Conclusion. 
I can correctly predict whether a business listed on Yelp is open or closed, around 80 percent of the time. This is important as I can use this model to consult or inform critical business decisions that can influence optimal location, desired amenities, and hours of operation to create the best environment in which a business can succeed. 
