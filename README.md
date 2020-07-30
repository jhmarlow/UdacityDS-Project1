# Airbnb Seattle Analysis Blog Post
### Udacity DataScience NanoDegree Project 1

This repo contains the code used to produce the data analysis and interactive visualistions for a [blog post](https://medium.com/p/438db3d27c4f/edit) on Medium.

## Business Understanding

Airbnb has become the go-to marketplace when trying to find a place to stay. However, it can sometimes be overwhelming when faced with a mass of choices, and numerous factors to filter against. In this article, we take a look at Seattle's Airbnb ecosystem. Looking at how location can affect price, how prices change throughout the year, as well as the type of listings available these neighbourhoods.

**Questions**:
1. How does distance to the city centre affect listings?
2. What is the best time of year to go?
3. What type of listings are available in Seattle?
4. How are the listings managed in Seattle?
5. Can we predict the Airbnb prices using factors assessed?

## Data Understanding

The data was provided from the Kaggle project (https://www.kaggle.com/airbnb/seattle/data). This was taken from the opensource data provided by airbnb (http://insideairbnb.com/get-the-data.html)

The data made available was:
- Calendar.csv - listing prices across the year 
- Listings.csv - property listings available through Airbnb in Seattle in 2016
- Reviews.csv - reviews left for listings

## Modelling and Preparation

Data cleaning was performed, including:

- Cleaning strings of unwanted characters
- Onehot encoding to handle categorical variables
- Scaling for ML model
- GPS distance calculation using the Haversine Formula 
    - Ref: https://www.kite.com/python/answers/how-to-find-the-distance-between-two-lat-long-coordinates-in-python
- Reviewing data skew

**ML Features**:
- neighbourhood_group_cleansed
- host_is_superhost
- room_type
- bathrooms
- bedrooms
- beds
- review_scores_rating
- review_scores_cleanliness
- review_scores_location
- review_scores_value
- reviews_per_month
 
 **Target**:
 - price

## Modelling

As part of the evaluation a simple Linear Regression Machine Learning Model was created using the sklearn library to assess the usage of reviews to predict the price associated with the listing.

R^2 score of 54%

## Evaluation

To review the output please look at the medium article here.

## Deployment
- Tools
    - Jupyter Notebooks: used as datascience analysis
    - pandas: data manipulation
    - Plotly: Interactive plots deployed to Medium article
        - Ref: https://towardsdatascience.com/how-to-create-a-plotly-visualization-and-embed-it-on-websites-517c1a78568b
    - Sklearn learn: Linear regression Model
    
[test](images/review_scores_distribtion.png)

# Acknowledgement
 This was completed as Project 1 of Udacity's Datascience Nanodegree
