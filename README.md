# IBM-Applied-Data-Science-Capstone
This project will be making calls to the Foursquare API to pull location data, and using the data to create meaningful business insights and geospatial visualizations

# Introduciton/Identifying a Business Problem
The corporate office of a growing chain of coffee shops is looking to expand. They plan to open a new store in Chicago, IL, but cannot determine the most optimal location for their new store. Our shareholders are looking for data-driven insights to fuel this site selection process. The goal of this project will be to identify the most optimal zip code for a new coffee shop based on trends in location data.

# Data
I will call the Foursqaure API to fetch this data. All of my analysis will be based on indicators driven from the Foursqaure dataset. Some factors to keep in mind when selecting what data to use in analysis for this use case:

1. Number of competing coffee shops in each area (we will use zip codes).
2. Type of attractions adjacent to established, successful coffee shops.

# Methodology
I will begin with a K-Means cluster on Chicago zip codes based on their most high-traffic venues. From these clusters, we can limit zip codes to the cluster with the highest number of successful and established coffee shops. From that cluster, we can filter out zip codes that already have a high-traffic coffee shop. Based on the nearby attractions and geographic location of the remaining zip codes, we can explore that data to determine our most optimal location.

# Results
After filtering out zip codes in the targeted cluster with an existing high-traffic coffee shop, we were left to select from 6 zip codes. Of these, zip code 60605 was not only the most central location, but also the most high-traffic due to the nearby museums, aquarium, gift shop, and many more top-notch attractions.

# Discussion
I considered performing another cluster on the remaining 14 zip codes, however, our folium map clearly showed that some zip codes were much farther out from the heart of Cluster 0 (Downtown Chicago). From the remaining 6, it was clear that zip code 60605's nearby venues were the most high-traffic and similiar to Chicago's greatest cafes.

# Conclusion
The purpose of this project was to identify the most optimal zip code for a new coffee shop based on trends in location data. By targeting the cluster with the highest desnity of well-established coffee shops, we were able to identify the best district for our new location. And after removing the zip codes with a pre-existing high-traffic coffee shop, we were able to narrow down the optimal location based on the nearby attractions of the remaining zip codes (i.e. Museums, Acquarium, etc.). This project is a great display of the power to be harnessed with K-Means clustering, geospatial visualizations, and real-time API's such as Foursquare's. 
