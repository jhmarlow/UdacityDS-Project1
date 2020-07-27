# Airbnb Seattle Analysis Blog Post
### Udacity DataScience NanoDegree Project 1

This repo contains the code used to produce the data analysis and visualistion in this (https://medium.com/p/438db3d27c4f/edit) Medium article.

## Business Understanding

The purpose of this analysis was to explore how the airbnb prices are affected across neighbourhoods. it also looks at how the properties are being managed by the hosts and can be seen that particular neighbourhoods are container owners that have multiple properties available all year round to make a profit. 

**Questions**:
1. How does distance to the city centre affect listings?
2. What is the best time of year to go?
3. What type of listings are available in Seattle?
4. How are the listings managed in Seattle?
5. Can we predict the Airbnb prices using factors assessed?

## Data Understanding

The data was provided from the Kaggle project (https://www.kaggle.com/airbnb/seattle/data). This was taken from the opensource data provided by airbnb (http://insideairbnb.com/get-the-data.html)

The data made available was:
Calendar.csv - Seattle Airbnb prices across the year
Lisitngs.csv - the listings available in Seattle in 2016
Neighbourhoods.gejson -  geojson for neighbourhood zones

## Modelling and Preparation

Data cleaning was performed, including:

- Cleaning strings of unwanted characters
- Datasets where joined
- GPS distance calculation using the Haversine Formula (https://www.kite.com/python/answers/how-to-find-the-distance-between-two-lat-long-coordinates-in-python)

## Modelling

As part of the evaluation a simple Linear Regression Machine Learning Model was created to assess the usage of Reviews to predict the price associated with the listing.

## Evaluation

It can be seen that the neighbourhood stayed in affects the price.

![alt text](images/dist.png)

Distance to city centre affects price.

![alt text](images/monthly_prices.png)

## Deployment
- Tools
    - Jupyter Notebooks: used as datascience analysis
    - pandas: data manipulation
    - Plotly: Interactive plots deployed to Medium article following (https://towardsdatascience.com/how-to-create-a-plotly-visualization-and-embed-it-on-websites-517c1a78568b)
    - Scikit learn: Linear regression Model


# Acknowledgement
 This was completed as Project 1 of Udacity's Datascience Nanodegree
