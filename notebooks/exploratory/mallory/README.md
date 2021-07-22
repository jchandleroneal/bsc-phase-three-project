# Chocolate Rating Analysis


## Authors:
Mallory Wilson, Dorothy Alexander, James Chandler O'Neal


## Overview
A chocolate company wants to find out why some of their  dark chocolate bars sell and why some of it does not sell as well. This project will analyze how different features of dark chocolate will affect the rating of the chocolate. During this project, we examined the relationship between different features and the rating of the chocolate bars to see which features have an impact on the rating of the chocolate.  

## Business Problem
A dark chocolate bar company notices that some of their chocolates sell out much faster than others, and some never sell. They want to find out why some of their chocolate sells out and why some does not. In order to do this, the company needs to find out what features of a chocolate bar make it better than others. We want to know which features have an impact on how much people like that chocolate. 


### Data Understanding
For this project, we used the Flavors of Cacao Dark Chocolate Bar Rating dataset. We had to webscrape the data from the website and put it in jupyter lab so that we could manipulate it in different ways. This dataset is mostly categorial and included features such as where the chocolate was made and sold, the cocoa percent in the chocolate, and the most memorable characteristics of individual chocolate bars. In order to understand the data, we first had to investigate which features had an impact on our target, the rating of the chocolate. Most of the data in our dataset was categorical data. 


### Data Preparation
Once we understood the data that we were working with, we went through and cleaned the data by imputing null values a. We had to convert all of the categorial columns into bins  containing "a,b,c" or '0,1'. We had to do this in order to  model since you cannot perform models on catergorial data. We also had to one hot encode some of the data. Our target feature, rating, was originally on a scale from 1 to 5 but we transformed it to  0's and  1's where anything rated 3 and below is "bad", therefore it  is assigned to  0 and anything about 3 is "good", and  will be assigned to 1. 


## Modeling


## Results


## Conclusions


## Next Steps


## Repository Structure


