# Chocolate Rating Analysis

![features bar plot](./images/main_cover.jpg)

---
## Authors:

 James Chandler O'Neal, Mallory Wilson, Dorothy Alexander
---

## Overview

This project focused on creating a model that could determine the factors with the largest role in producing a highly rated chocolate bar. The project used The Flavors of Cacao dataset containing 2,236 rows (items) and 19 columns (features) which, through exploratory data analysis and preprocessing, we then consolidated to 2231 rows, and 8 features. This model could be useful for Hu Kitchen to create a new chocolate bar with a high rating (above 3.0 out of 4.0).  

---

## Business Problem
Hu Kitchen has sought out for a model that would offer them insight in creating a highly rated chocolate bar.Hu Kitchen may benefit from focusing their funding on cocoa percentage, ingredients, bean origin, and partnering with other chocolate producers to create a new chocolate bar with a high rating. This project used F-1 Score for its metric as it does not consider false negatives (predicting a negative rating when it was actually positive) a higher priority and vice versa - rather, it weighs them equally.

---

## Data 

The project used The Flavors of Cacao dataset which included 19 features; some of which were the percent of cocoa, the most memorable characteristic, the company location, where the bean is from, the rating of the chocolate, and the different ingredients that were used.     

---

## Methods

This project utilized logistic regression, decision tree classifiers, random forest classification models, and pipelines to determine the best possible predictions. The Random Forest Classifier outperformed the other models validation sets and predicted the rating of the final test set of the given chocolate bar features with an accuracy of 79.1%. In order to gain these results, the Random Forest model was first run through a pipeline that performed SMOTE to deal with the imbalance within the dataset and finally ran a GridSearchCV to to establish the best hyperparameters (criterion, max_depth, max_leaf_nodes, and class_weight) to tune the model with.

---

## Results


The five most prominent features in creating a highly rated chocolate bar resulted in the following:

1. Company manufacturer - Bin D (company manufacturers with the greatest number of positive ratings), 
2. Ingredient Combinations - B, S, C (bean, sugar, cocoa butter), 
3. Company manufacturer - Bin C (company manufacturer with the second greatest number of positive ratings), 
4. Specific Bean Origin - 3 (bean growth origin with the resulted highest weighted ratings), 
5. Ingredient Combination - B, S, C, V, L (Bean, Sugar, Cocoa butter, Vanilla, Lecithin).

![features bar plot](./images/impactful_features.png)

---

The following companies were bucketed according to their indexes (row locations). While "d" had the largest number of companies, it also had the least amount of negative ratings making it a valuable group of comapanies. 

* Both negative and positive ratings were grouped using values of 1 for positive (rating > 3) and 0 for negative (rating < 3). The number of negative rating occurances appear in blue and positive in orange. 

![manufacture ratings](images/manufacture_ratings.png)
 
---

While "d" proved to be valuable in resulting in a positive rating, it made more sense to further classify it by taking the top 5 performing companies from group "d". Idilo, Cacao Sampaka, Soma, Brasstown aka It's Chocolate, and Ritual outperformed the other companies in terms of positive ratings with a mean average rating above 3.5.

![top companies](images/top_5_companies.png)

---


Portrayal of the 9 ingredients that produced the highest ratings. In terms of feature importance, B, S, C (bean, sugar, cocoa butter), or B, S, C, V, L (Bean, Sugar, Cocoa butter, Vanilla, Lecithin) proved to be the most impactful in towards producing a highly rated chocolate bar.

![ingredients list](images/ingredients_list.png)

---

## Conclusions

* Hu Kitchen should focus their funding on partnering with one of the following companies to create their new chocolate bar: Idilo, Cacao Sampaka, Soma, Brasstown aka It's Chocolate, or Ritual. 

* They should also use ingredient combinations of either B, S, C (bean, sugar, cocoa butter), or B, S, C, V, L (Bean, Sugar, Cocoa butter, Vanilla, Lecithin).

* Lastly, Hu Kitchen should also use a bean growth origin from one of the numerous groups (classified as group C) with the highest weighted averages for rating such as the Dominican Republic. 

---

## Next Steps
The next steps that should be taken would be to look into other kinds of chocolate, such as milk chocolate since this database only contained dark chocolate. Also, creating a Graphical User Interface(GUI) would be helpful for companies to input features of chocolate they are looking at and the GUI will produce a prediction of what the rating of their chocolate would be. One last step to take would be to look into how extra ingredients, such as nuts or caramel affect the rating of the candy bar. 

---

## For More Information
Please review the full analysis via [Jupyter Notebook](./notebooks/final_notebook.ipynb) or [Powerpoint](./Chocolate_Rating_Analysis.pdf).

For any additional questions, please contact James Chandler O'Neal & jchandleroneal@gmail.com, Mallory Wilson & mallorye1103@gmail.com, Dorothy Alexander & dorothy408@gmail.com 

---

## Repository Structure
```
├── README.md                               <- The top-level README for reviewers of this project
├── final_notebook.ipynb                    <- Narrative documentation of analysis in Jupyter notebook
├── presentation_Chocolate_Analysis.pdf     <- PDF version of project presentation
├── data                                    <- Both sourced externally and generated from code
│   ├── EDA.csv
│   └── chocolate.csv
├── notebooks 
│   ├──exploratory
│   └── final_notebook.ipynb
└── images                                  <- All photos used for README.md
    ├──cover chocolate 
    ├──impactful features
    └──...
