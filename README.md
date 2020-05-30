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

Next step was visualizing all neighborhoods in a map, so I used Folium to add markers for each neighborhood thorugh it's coordinates and generate the map.

![](images/map1.png)

Now, proceeding to gathering data about the venues, Foursquare API was utilized to search for maximum 100 venues in a certain radius from a neighborhood, then I have the name, category and coordinates of each venue as seen in the dataframe below and example for one neighborhood.

![](images/df2.png)

It takes a while to extract all venues for all the neighborhoods, it resulted in 8992 venues in total.

![](images/df3.png)

The next part was preparing the data to run K-Means Clustering algorithm, so I used One-Hot Encoding to have a column for each category and group it by the neighborhood such as in the dataframe below.

![](images/df4.png)

Finally I could run the clustering algorithm in which I considered that I wanted to cluster the neighborhoods into three clusters, as we can see in the map below.

![](images/map2.png)

# Results


