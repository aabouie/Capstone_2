# Project: Predicting Airbnb Listing Price in Austin, TX

![](img/Austin_Airbnb.JPG)

Airbnb is an online marketplace that connects people who want to rent out their homes with people who are looking for accomodations in that area. Airbnb currently covers more than 100,000 cities and 220 countries worldwide. The company's name comes from "Air Mattress B&B".










The dataset includes Airbnb availble units, locations, availability data, etc.



## Web Scraping
In this project, I scraped the Airbnb website to get the details of all available units in Austin, TX area. It's worth to mention that the units URLs were obtained from the available records on Insideairbnb.com website. After scraping the Airbnb website, the details of 10272 units with more than 80 features were obtained. You can find the scraping code in the following directory: SRC/Airbnb_Scraping.ipynb


## EDA Analysis











### Features
Features are chosen only if they were informative and are likely to correlated with the price label. Therefore, I eliminated features like id, host_id, neighborhood description which did not have an impact on the listing price. In addition, I removed some of the other features such as longitude and lagitutude as I was mainly using zipcode as the feature.

* Label


* Continous features



* Categorical features:


* Text features:


* Date features: 


Final Features that were included in the model are:
* host_is_superhost
* host_listings_count
* host_total_listings_count
* Accommodates
* Number of bedrooms
* Number of beds
* Number of bathrooms
* Minimum number of nights of reservation
* Maximum number of nights of reservation
* Availability of the unit in the next 90 days
* Total number of reviews
* Total number of reviews over the last 30 days
* Whether the unit is instantly bookable or not
* How long the host has joined Airbnb
* Whether the availble room is private or shared
* Whether the entire house is available or not
* Cleanliness score
* Accuracy score
* Communication score
* Checkin score
* Value score
* Available Amenities:
    * Pool 
    * TV 
    * Washer 
    * Dryer
    * Balcony
    * Private entrance
    * BBQ grill
    * Hot tub
* Single level home
* Five areas in Austin with the following zip codes:
    * 78702
    * 78703
    * 78704
    * 78734
    * 78746




![](img/Correlation.png)





## Data Insights


| Command | Description |
| --- | --- |
| ![](img/Room_type.png) | ![](img/House_type.png) |



![](img/Room_type.png)



![](img/House_type.png)


![](img/Location.png)


![](img/Price_vs_guest.png)


![](img/Price_vs_guest.png)

![](img/Price_vs_superhost.png)



![](img/Owners.png)


![](img/host_joined.png)



![](img/Airbnb_prices.png)





## ML WORK



![](img/residuals.png)



Random Forest
![](img/rf_GINI_Importance.png)

![](img/rf_permutation.png)

![](img/rf_test.png)

![](img/rf_training.png)



GB
![](img/GB_GINI.png)
TEST
![](img/GINI_Test.png)
TRAIN
![](img/GINI_Train.png)


![](img/Test_gb_less_800.png)


## Future Work






## Acknowledgments
I greatly appreciate Galvanize instructors, Juliana Duncan and Dan Rupp, for their valuable comments during this project. I would also like to thank Wing Lau for her insight through this project.



![](images/Introduction.png)

<img src="images/Workflow.jpg" width=800 height = 400>