# Project: Predicting Airbnb Listing Price in Austin, TX

![](img/Austin_Airbnb.JPG)

Airbnb is an online marketplace that connects people who want to rent out their homes with people who are looking for accomodations in that area. Airbnb currently covers more than 100,000 cities and 220 countries worldwide. The company's name comes from "Air Mattress B&B".

Although Airbnb and some other 3rd party website (e.g., beyondpricing.com) are also availble, however, the hosts still need to specify their expected daily price, and the algorithm can change the base price based on several factors such as seasonaility, day of the week, and any special events/conferences.

Airbnb pricing is significantly important specially as competitiveness increases and more units become availble for rental on Airbnb, Hence even small difference in prices can make a big difference. In addition, it is importnat to understand the guests need to obtain more review, higher score, and provide better amenities.

This projects aims to solve this problem by predicting the base price of Airbnb units in Austin, using machine learning algorithms. In the following section, I'm going to describe the exploratory data analysis, followed by building different models to predict Airbnb prices.


## Web Scraping
In this project, I scraped the Airbnb website to get the details of all available units in Austin, TX area. It's worth to mention that the units URLs were obtained from the available records on Insideairbnb.com website. Then, Selenium and BeautifulSoup were used to scrape the required data from each Url, followed by storing the data in Mongo database.
After scraping the Airbnb website, the details of 10272 units with more than 80 features were obtained. You can find the scraping code in the following directory: SRC/Airbnb_Scraping.ipynb

## EDA Analysis




According to data from Beyond Pricing, someone with a FLAT pricing plan can stand to gain as much as 43% on revenues.  Even very experienced hosts who keep diligent market data and track competitive pricing regularly can expect to gain at least 10% to their revenues.

It’s not easy to price your Airbnb unit on your own and it takes up quite a bit of time and effort that you might not have.

Having a partner like Beyond Pricing that can automatically track all the relevant data for you and adjust your pricing optimally to get you more profits is worth considering if you want more bookings during low season and higher booking rates during high season.


Many Airbnb hosts, particularly new and less experienced ones, will set a baseline price for their unit and then just forget about it.  This is a perfect way to miss out on bookings and leave profits on the table.

Let’s look the example below with three different hosts, each holding a flat pricing throughout the year.



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


The following figure shows the correlation heat map for some of the important features in the dataset. As can be seen, number of beds, bedrooms, bathrooms, and accomodates have relatively high positive impact on the Airbnb listing price.

![](img/Correlation.png)


## Data Insights
In this section, I explored the data in more details to get more understanding of the correlation



![](img/Room_type.png)



![](img/House_type.png)

In terms of location of Airbnb units, 18 out of 20 locations with highest Airbnb units are located close to the downtown area and zilker part where most of the music and film festivals are being held. For people who are not familiar with Austin area, East downtown is one of the most fast growing areas in Austin.

![](img/Location.png)


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


| Feature Importance in Random Forest | Feature Importance in Gradient Boosting |
| --- | --- |
| ![](img/rf_GINI_Importance.png)| ![](img/GB_GINI.png) |



## Future Work






## Acknowledgments
I greatly appreciate Galvanize instructors, Juliana Duncan and Dan Rupp, for their valuable comments during this project. I would also like to thank Wing Lau for her insight throughout this project.



![](images/Introduction.png)

<img src="images/Workflow.jpg" width=800 height = 400>