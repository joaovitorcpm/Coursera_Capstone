# Coursera_Capstone

# Introduction
The Goal of this study is to enable a restaurant chain to plan their investiment and open new restaurants in my city, Belo Horizonte - Minas Gerais - Brazil. Belo Horizonte is the capital of the state and one of the most populated cities in Brazil, having a population of 2,5 million people in the city, but almost 5 million when adding population from the nearby cities. However, the city is formed by different types of neighborhoods in which rich and poor people live. This way, it is important to evaluate the characteristics of these neighborhoods to determine in which one should they open their first restaurant.

# Data
The data regarding the list of neighborhoods and their respective boroughs will be extracted from https://pt.wikipedia.org/wiki/Lista_de_bairros_de_Belo_Horizonte, see below the map of boroughs in Belo Horizonte.
![](images/BH.png)

Then, I'll extract geographical coordinates for each neighborhood usigin Geopy API and then get the venues of each neighborhood with Foursquare API.

# Methodology
First I gathered the list of all neighborhoods of Belo Horizonte at WikiPedia and used GeoPy to get latitude and longitude for each neighborhood to have a dataframe as below.
![](images/df1.png)
