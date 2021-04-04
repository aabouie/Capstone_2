# Project: Predicting Airbnb Listing Price in Austin, TX
![](images/Introduction.png)

<img src="images/Workflow.jpg" width=800 height = 400>




![](img/Austin_Airbnb.JPG)

The dataset includes Airbnb availble units, locations, availability data, etc.



## Web Scraping





## EDA Analysis











### Features
Features are chosen only if they ware informative and are likely to correlated with the price label. Therefore, I eliminated features like id, host_id, which appear to be noise. In addition, I removed some of the other features such as longitude and lagitutude.

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




