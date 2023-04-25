# nosql-challenge
<p align="center">
<img width="450" height="300" src="https://www.foodsafetynews.com/files/2019/04/dreamstime_food-hygiene-rating-scheme-fsa.jpg">
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
        Leo's Bar & Grill,  Royal Ribs, Great Hallingbury Manor Hotel, The Dog And Duck, Oriental Cottage </i></br>
        
<b>2. Which establishments in the City of London Authority have an overall rating of 4 or above?</b> </br>
        This was answered by querying to return any establishment that contained "London" in the Local Authority field, and had a rating value of 4 or above. This retured the following restaurants:</br>
        <i> Charlie's, Mv City Cruises Erasmus, Benfleet Motor Yacht Club, Coombs Catering t/a, The Lock and Key,
        Tilbury Seafarers Centre, Mv Valulla, Tereza Joanne, Brick Lane Brews, The Nuance Group (UK) Limited,
        WH Smith, City Bar & Grill, Jet Centre, Caffè Nero, Mv Sunborn Yacht Hotel,
        Good Hotel London, La Nonna lina, Wake Up Docklands Limited, MV Venus Clipper, MV Typhoon clipper,
        MV Moon clipper, MV Jupiter clipper, MV Monsoon clipper, MV Tornado clipper, MV Meteor clipper, 
        MV Mercury clipper, MV Cyclone clipper, MV Galaxy clipper, MV Sun clipper, MV Hurricane clipper,
        Mv Storm Clipper, MV Neptune clipper, MV Aurora clipper, Canary Wharf 1V </i></br>

<b>3. What are the top 5 establishments with a RatingValue of 5 nearest to the new restaurant added during data cleaning?</b></br>
        This was answered by querying for a Rating of exactly 5 within 0.1 degrees of both the latitude and longitude of our new Penang Flavours restaurant. The returned list of establishments can be seen here:
        <i> - Fineway Cash & Carry
        - Premier Express
        - The Plumstead Pantry
        - Everest Stores Ltd
        - TIWA N TIWA African Restaurant Ltd </i>

4. How many establishments in each Local Authority area have a hygiene score of 0? 
