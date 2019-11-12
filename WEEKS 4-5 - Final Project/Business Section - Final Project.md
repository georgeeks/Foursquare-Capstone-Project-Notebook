
#### COURSERA-IBM - APPLIED DATA SCIENCE - FINAL PROJECT

# Business Section

# PHARMA FRANCISE  - new locations in Paris
###  A new pharmacy chain - opportunity solutions for building location

![](https://github.com/georgeeks/Foursquare-Capstone-Project-Notebook/blob/master/WEEKS%204-5/Paris%20overview.jpg)"Paris overview"


## Business overview
Pharmacies are together with hospitals and medical clinics, essential institutions for the health of the population. In addition to the social good, pharmacies are also a successful business.
We have been approached by a new pharma investor to present an optimal solution for the placement of 10 new pharmacies in a European capital.  

## Task overview  
Our task is to propose the optimal locations  
We have chosen as optimal the points that satisfy the following requirements, in the following order of importance:
### Main criteria:
- Neighborhood of hospitals or medical clinics
- Neighborhood of malls or areas with high pedestrian traffic
- The greatest distance from the existing pharmacies
### Secondary criteria:
- Neighborhood of public transport
- Hours of operation of public locations in the area  

# Data Section


### Method: 
- Geotagging
- Multiclass Classsification
- Clustering  

![](https://github.com/georgeeks/Foursquare-Capstone-Project-Notebook/blob/master/WEEKS%204-5/paris_map.jpg)
 
### Methodology:
   - Understanding investor intention - prerequisite
   - Understanding the importance of optimal conditions of the localities - prerequisite
   - Defining a large area - the city, the country
   - Establishing the layers according to the investor criteria
       - areas with heavy pedestrian traffic like large intersections, malls, markets etc. Foursquare request  
       - hospitals, existing clinics. Foursquare request
       - pharmacies in the area. Foursquare request
       - operating hours. Foursquare request
   - Data Exploration, Feature engineering for optimal definition of features (criteria)
   - Classification of layers  
   - Clustering according to criteria
       - of traffic
       - of distance
           - proximity - hospitals, markets
           - away - existing pharmacies
   - View with Folium Maps
   - Presentation of the conclusions to the investor
     ... Get payment ... and congrats!

### Tools: 
 - Anaconda Python Environment
 - Forsquare API
 - Folium
### Techniques: 
 - API Request for layer defining
 - Data Exploration and Feature Engineering for Point Setting
 - Folium Map View
 - Sklearn's k-means Clustering