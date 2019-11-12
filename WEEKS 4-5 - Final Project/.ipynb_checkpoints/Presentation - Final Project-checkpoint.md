
#### COURSERA-IBM - APPLIED DATA SCIENCE - FINAL PROJECT

# PHARMA FRANCISE  - new locations in Paris
###  A new pharmacy chain - opportunity solutions for building location

![](https://raw.githubusercontent.com/georgeeks/Foursquare-Capstone-Project-Notebook/master/WEEKS%204-5%20-%20Final%20Project/project_images/Paris%20overview.jpg) "Paris overview"


## Introduction 
### Business overview
Pharmacies are together with hospitals and medical clinics, essential institutions for the health of the population. In addition to the social good, pharmacies are also a successful business.

<img src="https://github.com/georgeeks/Foursquare-Capstone-Project-Notebook/WEEKS%204-5%20-%20Final%20Project/project_images/GlobalWellnessEconomy2017_bubblechart-1024x780.jpg" width="800" />

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
    
![](https://github.com/georgeeks/Foursquare-Capstone-Project-Notebook/blob/master/WEEKS%204-5%20-%20Final%20Project/project_images/France_assembly_vote.png?raw=true"France regions") 

    
   
  
   
   
   - Establishing the layers according to the investor criteria
       - areas with heavy pedestrian traffic like large intersections, malls, markets etc. Foursquare request  
       
 
       - hospitals, existing clinics. Foursquare request
       
       
       - pharmacies in the area. Foursquare request
           
       
       
   - Data Exploration, Feature engineering for optimal definition of features (criteria)
   - Classification of layers  
   - Clustering according to criteria
       - of traffic
       - of distance
           - proximity - hospitals, markets
           - away - existing pharmacies
   - View with Folium Maps
   - Presentation of the conclusions to the investor
   
## Results section where you discuss the results.
## Discussion section where you discuss any observations you noted and any recommendations you can make based on the results.
## Conclusion section where you conclude the report.

