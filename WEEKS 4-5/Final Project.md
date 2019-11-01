
#### COURSERA-IBM - APPLIED DATA SCIENCE - FINAL PROJECT

# PHARMA FRANCISE  - new locations
###  A new pharmacy chain - opportunity solutions for building location


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

## Methodology, Tools and Techniques  

### Method: 
 - Geotagging, 
 - Multiclass Classsification, 
 - Clustering  
 
### Methodology:
1. Understanding investor intention - prerequisite
2. Understanding the importance of optimal conditions of the localities - prerequisite
3. Defining a large area - the city, the country
4. Establishing the layers according to the investor criteria:
a. areas with heavy pedestrian traffic - large intersections, malls, markets etc. - Foursquare request
b. hospitals, existing clinics - Foursquare request
c. pharmacies in the area - Foursquare request.
d. operating hours - Foursquare request
5. Data Exploration, Feature engineering for optimal definition of features (criteria)
6. Classification of layers
7 . Clustering according to criteria:
a. of traffic
b. from a distance:
- proximity - hospitals, markets
- away - existing pharmacies
8. View with Folium Maps
9. Presentation of the conclusions to the investor
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