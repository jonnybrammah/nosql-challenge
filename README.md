# nosql-challenge
<p align="center">
<img width="400" height="300" src="https://www.foodsafetynews.com/files/2019/04/dreamstime_food-hygiene-rating-scheme-fsa.jpg">
</p>

## Project Description

The goal of this project was to evaluate some of the UK Food Standards Agency ratings for restaurants in the UK for the food magazine, <i>Eat Safe, Love</i>. A json file containing the data on restaurants was imported to MongoDB using a command prompt window. From there, data cleaning and eventual data analysis were completed in a jupyter notebook using the PyMongo library.'

-----

### Table of Contents
1. [<b>Data Cleaning</b>](https://github.com/jonnybrammah/nosql-challenge/blob/main/README.md#data-cleaning)
2. [<b>Data Analysis</b>](https://github.com/jonnybrammah/nosql-challenge/blob/main/README.md#data-analysis)
-----

### Data Cleaning

<p align="center">
<img width="300" height="100" src="https://github.com/jonnybrammah/nosql-challenge/blob/main/Resources/Penang%20Flavours.png">
</p>

A new restaurant, Penang Flavours, was added to the collection, and then updated using the BusinessTypeID used by the data base. This restaurant was required for a future magazine article.

Some data stored in the dataframe was not in the correct datatype, so latitude and longitude were both converted to decimals, and the overall Rating of the resaturant was converted to an integer.

-----

### Data Analysis

The questions to be answered during the analysis of the data were: </br>
<b>1. Which establishments have a hygiene score equal to 20?</b> </br>
    This was answered by writing a query to return any establishment where the Hygiene score was exactly 20, and returned a list of 41 business, which can be vieweed here:</br>
      <i> The Chase Rest Home, Brenalwood, Melrose Hotel, Seaford Pizza, Golden Palace,
      Ashby's Butchers, South Sea Express Cuisine, Golden Palace, The Tulip Tree, F & S,
      Longhouse, Westview Playgroup Based At Downsview Comm Primary, Whatever The Weather Coffee, Kings Restaurant (Oriental), Xich Lo,
      Asian Supermarket Ltd: T/A Best Food Wine Ltd, Londis, Costcutter, La Simon Ltd, Caribiscus Ltd,
      Kennedy Fried Chicken, Gah Shing, A1 News & Wine, Cakes & Bakes, Sahajanand Catering Limited, Sisko Cafe,
      Magazin Romanesc Diana, Bali Maamalas, Angels Bakery, Nikkis Place Restaurant, Chicago 30,
      Samui Thai Restaurant, Pakhtoonkhwa Restaurant, New Happy Garden, Mummy Yum, Gospodina,
      Leo's Bar & Grill,  Royal Ribs, Great Hallingbury Manor Hotel, The Dog And Duck, Oriental Cottage
      </i>
2. Which establishments in the City of London Authority have an overall rating of 4 or above?
3. What are the top 5 establishments with a RatingValue of 5 nearest to the new restaurant added during data cleaning?
4. How many establishments in each Local Authority area have a hygiene score of 0? 
