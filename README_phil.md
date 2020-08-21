# Housing Market in King County

## Problem Statement:

As a Junior Data Scientist, I have been tasked with investigating house sales in the King County area and building a model to suggest home improvements in order to increase house value.

The following questions will be answered in this project:

* Which feature generates the best model, zip codes or sub regions?

* Does transforming the target value improve model efficiency?

* Which house attributes have a high impact in sale price and which attributes have the least/negative impact?

# Components:

* Jupyter Notebook - A well documented Jupyter Notebook containing any code I've written for this project and comments explaining it.

* Presentation - Short PowerPoint presentation, delivered as a PDF export, giving a high-level overview of your methodology and recommendations for non-technical stakeholders.

* Blog Post - Blog post found on this link (https://phillipojo24.github.io/linear_regression_model)

* Data - King County house sales dataset named 'kc_house_data.csv' and King County subregion by zipcode named 'SubRegZipCityNeighborhood.xlsx'

# Methodology:
On this project, the OSEMiN data science workflow was adopted.

OBTAIN - Understanding stakeholder requirements and sourcing data.

SCRUB - Identifying and removing null values, dealing with outliers, normalizing data, and feature engineering/feature selection

EXPLORE - Create visualizations to really get a feel for your dataset.

MODEL - Building and tuning models.

INTERPRET - Interpret the results of your model(s), and communicate results to stakeholders.

# Project Summary:

# Question 1 - Does the number of bedrooms have an high affect on sale price?

Intuitivly, looking at houses we assume that more bedrooms make the house more expensive. However after going through the data we see that this is not true. One-hot encoded the bedrooms to capture the categorical data.  

 <img src= "https://raw.githubusercontent.com/phillipojo24/dsc-mod-2-project-v2-1-onl01-dtsc-pt-041320/master/Screen%20Shot%202020-08-21%20at%2010.31.50%20AM.png">

 <img src= "https://raw.githubusercontent.com/phillipojo24/dsc-mod-2-project-v2-1-onl01-dtsc-pt-041320/master/Screen%20Shot%202020-08-21%20at%2010.34.48%20AM.png">

### Conclusion - The number of bedrooms did not seem to affect the sale price. However for a given house depending on its square-footage, note that adding an additional bedroom does not necessarily result in a a sale price increase. 

# Question 2 - Does the diffrenece in Zipcode affect sale price?

With the man diffrent zipcode values, we assumed that it will negativly affect the model. This prompted us to create Sub-Regions and group the zipcode into regions. However, this did not actually improve the model. 

<img src= 'https://raw.githubusercontent.com/phillipojo24/dsc-mod-2-project-v2-1-onl01-dtsc-pt-041320/master/Screen%20Shot%202020-08-21%20at%2010.35.21%20AM.png'>

### Conclusion- Grouping the zip codes into regions did not improve the model. However, by using the zip codes instead of the sub regions the model dramtically increased. Future analsis will invole seeing how the prices of house that are located to major sporting venues affect price. Also looking at ares that have been gentrifiied can show a depper insight into the affect of price.

# Question 3 - Which features have a high impact on sales price?

By standardizing the data, we are able to see the weight of each feature and how they affect price.

<img src= 'https://raw.githubusercontent.com/phillipojo24/dsc-mod-2-project-v2-1-onl01-dtsc-pt-041320/master/Screen%20Shot%202020-08-21%20at%2010.35.43%20AM.png'>

<img src= 'https://raw.githubusercontent.com/phillipojo24/dsc-mod-2-project-v2-1-onl01-dtsc-pt-041320/master/Screen%20Shot%202020-08-21%20at%2010.35.43%20AM.png'>

### Conclusion - From the results of our model, you can see that the least significant features are "Bedrooms" , "floors", and "Sqft of Lot". Most significant features are "Sqft Living", "View", "grade", and "Bathrooms". As a homeowner, if you want to increase the value of your house you should

    * Increase the living square footage of the house.
    * Imporve the overall grade of the house.
    * Adding a new bathroom will positivily affect price but dont go over board and exceed 4 bathrooms based on sqft living. Additional analysis will be to create a relationship between the number of bathrooms allowed and the total Sqft living and how that affects price. 
    * Renovating a house that has a condition score under "3" will help improve the sale price. If you plan to renovate, increase the total living square footage and investing in high quality materials.bathroom will positivily affect price but dont go over board and exceed 4 bathrooms based on sqft living. Additional analysis will be to create a relationship between the number of bathrooms allowed and the total Sqft living and how that affects price. 
    * Renovating a house that has a condition score under "3" will help improve the sale price. If you plan to renovate, increase the total living square footage and investing in high quality materials.

# Conclusion

## Question 1

* The number of bedrooms did not seem to affect the sale price. However for a given house depending on its square-footage, note that adding an additional bedroom does not necessarily result in a a sale price increase. 


## Question 2

* Grouping the zip codes into regions did not improve the model. However, by using the zip codes instead of the sub regions the model dramtically increased. Future analsis will invole seeing how the prices of house that are located to major sporting venues affect price. Also looking at ares that have been gentrifiied can show a depper insight into the affect of price.

## Question 3

* Based on the Regression Model, 
    * Don'ts
        * Adding a new bedroom does not guarantee that the house value will increase
        * Adding a new Floor does not guarantee that the house value will increase
    
    * Do's
        * Increase the living square footage of the house.
        * Improve the overall grade of the house.


```python

```
