# Capstone
How to pick a neighborhood to live in based on interests:

What is the best neighborhood to settle in knowing that our top 3 hobbies are :
reading books in parks, having coffee and going to restaurants

# Introduction
My project will help decide on a neighborhood to settle in based on a list of interests.
The audience is therefore people moving to Toronto, but the tool can easily be extended to other cities.

Let's say you have been tranfered to Toronto for a professional mission, and you are deciding which neighborhooh to live in. 
This project will be of great help picking the perfect neighborhood for you

# Data section
I will use the FourSquare API to collect data about venues in Toronto


# Methodology

For a specific City, I retrieve neighborhood data. I then fetch all venues for each neighborhood.
I do some statistics for each neighborhood : number of venues, most common type of venues, density etc..

I then define a list of interests (by default 3, here we are interested in : Coffee places , Parks, and restaurants)

based on above statistics I assign a score to each neighborhood, (indicatively 100% will be assigned if the 3 interests are among the top 5 type of venues in that neighborhood)

the output is a table of all neighborhood matching criterias, sorted based on the previously build score.
we also show the neighborhood on the map for a better visualization

Use Case Example : The individual looking to move in Toronto will prepare a list of venue types based on their interests.
we then retrieve all venues for each neighborhood we then classify them into categories and sort by density of such venues.

number of interests = 3
we will check the 5 most common type of venues and assign a score to each neighborhood based on that.
we will then come up with a score-based sorted list of  suggestions. 
we also show them in the map in order to better visualize the various neighborhood options

in this project we covered Toronto but we can easily extend the project to other cities

# Results
here is the output table as well as the map labelled with all the suggestions. the map was generated with folium.

# Discussion:
an interesting feature to add to the score would be the numbers of venues. 
The goal would be to distinguish more easily two neighborhood with the same most common venues based on the density.

# Conclusion:
This project can prove to be of great help for people looking for a neighborhood to live in. it is initially designed for Toronto but can be very easily extended to other city.
and based on the same logic we can offer the same solution to entrepreneurs looking to open up a business. they would be able to analyse easily which are the cities where there is less competition.
