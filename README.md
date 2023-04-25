# nosql-challenge
<p align="center">
<img width="400" height="300" src="https://www.foodsafetynews.com/files/2019/04/dreamstime_food-hygiene-rating-scheme-fsa.jpg">
</p>

## Project Description

The goal of this project was to evaluate some of the UK Food Standards Agency ratings for restaurants in the UK for the food magazine, <i>Eat Safe, Love</i>. A json file containing the data on restaurants was imported to MongoDB using a command prompt window. From there, data cleaning and eventual data analysis were completed in a jupyter notebook using the PyMongo library.'

-----

### Table of Contents
- 1. [Data Cleaning](https://github.com/jonnybrammah/nosql-challenge/blob/main/README.md#data-cleaning)
- 2. [Data Analysis](https://github.com/jonnybrammah/nosql-challenge/blob/main/README.md#data-analysis)
-----

### Data Cleaning

<p align="center">
<img width="300" height="100" src="https://github.com/jonnybrammah/nosql-challenge/blob/main/Resources/Penang%20Flavours.png">
</p>

A new restaurant, Penang Flavours, was added to the collection, and then updated using the BusinessTypeID used by the data base. This restaurant was required for a future magazine article.

Some data stored in the dataframe was not in the correct datatype, so latitude and longitude were both converted to decimals, and the overall Rating of the resaturant was converted to an integer.

-----

### Data Analysis
