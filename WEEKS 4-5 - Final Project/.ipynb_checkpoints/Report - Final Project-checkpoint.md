
#### COURSERA-IBM - APPLIED DATA SCIENCE - FINAL PROJECT

# PHARMA FRANCISE  - new locations in Paris
###  A new pharmacy chain - opportunity solutions for locations

![](https://raw.githubusercontent.com/georgeeks/Foursquare-Capstone-Project-Notebook/master/WEEKS%204-5%20-%20Final%20Project/project_images/Paris%20overview.jpg) "Paris overview"


## Introduction 
### Business overview
Pharmacies are along with hospitals and medical clinics, essential institutions for the health of the population. In addition to the social good, pharmacies are also a successful business.

![](https://raw.githubusercontent.com/georgeeks/Foursquare-Capstone-Project-Notebook/master/WEEKS%204-5%20-%20Final%20Project/project_images/GlobalWellnessEconomy2017_bubblechart-1024x780.jpg)
We have been approached by a new pharma investor to present an optimal solution for the placement of 10 new pharmacies in a European capital.
Anyway, the project may serve any other investment bussines for best suited locations.

### Task overview  
Our task is to propose the optimal locations for bussiness growth. We have chosen as optimal the points that satisfy the following requirements, in the following order of importance:
- Neighborhood of hospitals or medical clinics
- Neighborhood of malls or areas with high pedestrian traffic
- The greatest distance from the existing pharmacies
- Neighborhood of public transport

## Data used
- Pharma Global Bussines stats from @ https://globalwellnessinstitute.org/
- Pharma economic predictions from https://www.visualcapitalist.com/future-pharma-market/
- Demographic statistics of country, regions, capital, from The National Institute of Statistics and Economic Studies of France. (<a href='https://www.insee.fr/fr/statistiques/2119468?sommaire=2119504#departements'>L’Institut national de la statistique et des études économiques</a>\)  
(<a href='https://www.insee.fr/fr/statistiques/fichier/2387611/ensemble.xls'>France Department Population</a>) and   
(<a href='https://www.insee.fr/fr/statistiques/fichier/2387611/dep75.xls'>Paris (Ile-de-France)</a>)  
(<a href='https://en.wikipedia.org/wiki/%C3%8Ele-de-France#Population_density'>**Ile-de-France** population density</a>)  
(<a href='https://en.wikipedia.org/wiki/Quarters_of_Paris'>**Paris Quarters** population density</a>)  


- Geolocation coordinates of France, Ile-de-France, Paris and Arondisments through Fourquest API, GoogleMapAPI
- Venues data, geolocation, address location 

## Methodology:

### Methods: 
- Geotagging
- Multiclass Classsification
- Clustering  
### Tools: 
 - Anaconda Python Environment
 - Forsquare API
 - Folium
### Techniques: 
 - API Request for layer defining
 - Data Exploration and Feature Engineering for Point Setting
 - Folium Map View
 - Sklearn's k-means Clustering 

### Processing Stages
- Understanding investor intention - prerequisite
- Understanding the importance of optimal conditions of the localities - prerequisite
- Defining a large area - the city, the country
    - Import statistical data from The National Institute of Statistics and Economic Studies of France
![](https://raw.githubusercontent.com/georgeeks/Foursquare-Capstone-Project-Notebook/master/WEEKS%204-5%20-%20Final%20Project/project_images/France_assembly_vote.png)
    - Process data into Pandas DataFrame to show to most populated region
![](https://raw.githubusercontent.com/georgeeks/Foursquare-Capstone-Project-Notebook/master/WEEKS%204-5%20-%20Final%20Project/project_images/1124px-%C3%8Ele-de-France_region_locator_map2.svg.png)
![](https://raw.githubusercontent.com/georgeeks/Foursquare-Capstone-Project-Notebook/master/WEEKS%204-5%20-%20Final%20Project/project_images/France_regions.png)

![](https://raw.githubusercontent.com/georgeeks/Foursquare-Capstone-Project-Notebook/master/WEEKS%204-5%20-%20Final%20Project/project_images/Ils-de-France2.png)

    - The same for Paris and for Arondisments (Quarters)
![](https://raw.githubusercontent.com/georgeeks/Foursquare-Capstone-Project-Notebook/master/WEEKS%204-5%20-%20Final%20Project/project_images/Population_density_map_of_Paris_in_2012.svg.png) 
![](https://raw.githubusercontent.com/georgeeks/Foursquare-Capstone-Project-Notebook/master/WEEKS%204-5%20-%20Final%20Project/project_images/Paris_arondisments.png)
   - Establishing the layers according to the investor criteria
       - areas with heavy pedestrian traffic like large intersections, malls, markets etc. Foursquare request 
       
![](https://raw.githubusercontent.com/georgeeks/Foursquare-Capstone-Project-Notebook/master/WEEKS%204-5%20-%20Final%20Project/project_maps/map_quarters.png)
![](https://raw.githubusercontent.com/georgeeks/Foursquare-Capstone-Project-Notebook/master/WEEKS%204-5%20-%20Final%20Project/project_maps/paris_heatmap.png) 

   - hospitals, existing clinics. Foursquare request geolocation coordinates
![](https://raw.githubusercontent.com/georgeeks/Foursquare-Capstone-Project-Notebook/master/WEEKS%204-5%20-%20Final%20Project/project_images/hospitals_coordinates2.png) 
   - pharmacies in the area. Foursquare request geolocation coordinates
       
![](https://raw.githubusercontent.com/georgeeks/Foursquare-Capstone-Project-Notebook/master/WEEKS%204-5%20-%20Final%20Project/project_maps/paris_heatmap_hp.png)
       
   - Data Exploration, Feature engineering for optimal definition of features (criteria)
![](https://raw.githubusercontent.com/georgeeks/Foursquare-Capstone-Project-Notebook/master/WEEKS%204-5%20-%20Final%20Project/project_images/Venues_cat.png)
   - Classification of layers  
   - Clustering according to criteria
       - of traffic
       
![](https://raw.githubusercontent.com/georgeeks/Foursquare-Capstone-Project-Notebook/master/WEEKS%204-5%20-%20Final%20Project/project_maps/Paris_cluster1.png)
       
![](https://raw.githubusercontent.com/georgeeks/Foursquare-Capstone-Project-Notebook/master/WEEKS%204-5%20-%20Final%20Project/project_maps/paris_clustered_venues_map.png)

## Results

We have delimited special area for new locations in proximity to most populated area of the city, nearest to hospitals, restorants, markets and transport means.

![](https://raw.githubusercontent.com/georgeeks/Foursquare-Capstone-Project-Notebook/master/WEEKS%204-5%20-%20Final%20Project/project_maps/center_clusters_map.png)

   - View with Folium Maps
   
![](https://raw.githubusercontent.com/georgeeks/Foursquare-Capstone-Project-Notebook/master/WEEKS%204-5%20-%20Final%20Project/project_maps/Final_map.png)
   - Presentation of the conclusions to the investor
   
## Conclusion 

The project goes through the process of identifying the business problem, specifying
the data required, extracting and preparing the data, performing machine learning by clustering and provides accurate recommendations to the investors regarding the best locations for a new pharmacies chain. 
The most populated and most commercial interesting areas are in the center of the city, providing a grate economical oportunity. 
