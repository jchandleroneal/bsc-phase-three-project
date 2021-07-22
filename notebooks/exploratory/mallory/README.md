# Chocolate Rating Analysis


## Authors:
Mallory Wilson, Dorothy Alexander, James Chandler O'Neal


## Overview
A chocolate company wants to find out why some of their dark chocolate bars sell and why some of it does not sell as well. The focus  of this project is to analyze different features that go into a high rated chocolate bar. The project observed the Flavors of Cacao Dark Chocolate Dataset that contained information on the company location, bean origin, cocoa percent, ingredients, memorable characteristics, and rating. The categorical features were transformed by one hot encoding. This analysis could be useful for chocolate companies to determine what goes into a high rated chocolate bar.  


## Business Problem

A dark chocolate bar company notices that some of their chocolates sell out faster than others, and some never sell.  Chocolate  companies may be able to focus their funding on aquiring beans from certain countries or on beans with a medium level cocoa percent  in order to improve sales. In order to determine the reasoning behind these outcomes, the company needs to find out what features of a chocolate bar make it better than others. The goal of this project was to predict the most valuable features that go into a high rated chocolate bar. 


### Data Understanding/Preparation
The Flavors of Cocoa dataset contained multiple columns that could have an impact on our target, what the rating of a chocolate bar is.  


## Methods
This project uses different forms of modeling and inferential analysis, in order to find relationships between different chocolate variables and features. The first thing done was turning all of the categorical data into 0's and 1's so that they could be put into model's. The project began with a baseline logistic regression model, then some decision tree models, and a random forest classifier. A Grid Search was performed to find out which hyperperameters worked best for the models. These models were then tuned with different hyperperameters that were found. 

## Results


## Conclusions


## Next Steps


## Repository Structure


This project will analyze how different features of dark chocolate will affect the rating of the chocolate. During this project, we examined the relationship between different features and the rating of the chocolate bars to see which features have an impact on the rating of the chocolate. 
For this project, the Flavors of Cacao Dark Chocolate Bar Rating dataset was used. Webscraping was used to gather the data from the website and put it in jupyter lab so that it could be manipulate it in different ways. This dataset is mostly categorial and included features such as where the chocolate was made and sold, the cocoa percent in the chocolate, and the most memorable characteristics of individual chocolate bars. In order to understand the data, the project had to investigate which features had an impact on our target, the rating of the chocolate. Most of the data in our dataset was categorical data. 
Once we understood the data that we were working with, we went through and cleaned the data by imputing null values. We had to convert all of the categorial columns into bins  containing "a,b,c" or '0,1'. We had to do this in order to  model since you cannot perform models on catergorial data. We also had to one hot encode some of the data. Our target feature, rating, was originally on a scale from 1 to 5 but we transformed it to  0's and  1's where anything rated 3 and below is "bad", therefore it  is assigned to  0 and anything about 3 is "good", and  will be assigned to 1.