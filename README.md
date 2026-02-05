# Project title: "Reform Policies and it's effect AirBnB Listings Analysis."

# Introduction: 
<br>
During the 2015-2019 , there was a global reforms around many part of the worlds to address short term rental apps, websites, like Airbnb to address and in hopes of resolves the competitions between Airbnb rental and long term housing market. 

Some of the common points of these reform is about:
1. Setting limits on the amount of city properties can become short term rental.
2. Setting limits on the amount of times properties can be rents for.
3. Requires registrations, licensing and owners compliance with government policies.
4. Strengthens the city capability to enforces penalties for illegal and unregistered rentals.
5. Reform that aims to improves quality of lifes in neighbourhood effected by noise, tourism pressurement and comunity displacement.

Some of the finers details on why these reform matters include:

. Housing availability + Affordability: To reduces the conversions of long term housing to short term markets.

. Tourism balance: Keeping neighborhood livable for residents.

. Safety and standard: Ensuring guest accommodations meet local codes.

. Requirement for permits/registration.

. Night-cap limits on rentals.

. Host residency rules.

. Strict penalties and enforcement. 


# About the Project:
<br>
This project focus on these short-term rental reforms policies that effect AirBnB in particular, include:
. Numbers of available Airbnb properties and new hosting.
. How pricings of properties over time is effect by the reforms.


# Project Highlights:
<br>
This project aims to compare the analysis results between multiples cities from multiples economic zones with different economic conditions.

It's often under that the STR reform hits the West the hardest due to the developed economy and already high rental prices, compare to developing nations and zones, or weaker economic zone that may experiences these reform different.

Or at least that is the assumptions and data is waiting to proves or disproves that, data will also shown that even in Developed nations and their cities, different selection of measures would lead to different outcom.e

Because there are too many cities multiples regions of the worlds, three will be selected for Examination:
1. Paris From France.
2. Sydney From Australia.
3. Rio Dejaneiro from Brazil.

# Key Findings:
<br>

#### 1. Filter down the data to rows, where the data is only about the three cities aboves, and keep only the columns of "host_since", "neighbourhood", "city", "accommodates" and "price" in the table.

<img width="597" height="182" alt="image" src="https://github.com/user-attachments/assets/7992397e-9b28-4fba-a45e-313c535cd0fe" />

. The total data range is 27.9712 entries in total.

<img width="705" height="417" alt="image" src="https://github.com/user-attachments/assets/3d6ca73a-651c-4597-9e3f-b16328e8203b" />

. The seperation of the columns for the Paris Listing entry which yield in 64.690 entries.

<img width="707" height="415" alt="image" src="https://github.com/user-attachments/assets/52321737-0428-467a-8380-d71cc8ab3251" />

. Meanwhile the Sydney Listing entry yield in 33.630 entries.

<img width="706" height="412" alt="image" src="https://github.com/user-attachments/assets/79dc4b9b-88a9-4a95-965e-3ed11501a7c3" />

. The Rio Dejaneiro Listing have 26.615 entries.

#### 1B. Looking for missing values for all listings.

<img width="283" height="225" alt="image" src="https://github.com/user-attachments/assets/556859c2-3171-40d3-a46d-1633b3c5923f" />

<img width="297" height="236" alt="image" src="https://github.com/user-attachments/assets/bfa1a01c-1393-4207-933c-c91b6b88004c" />

<img width="360" height="252" alt="image" src="https://github.com/user-attachments/assets/e21535fe-ae9c-4126-8b7e-f6f7becb4f2e" />

. After removing invalid listings, Paris has 64,628 valid listings. 33 of them are missing host_since information, but all have valid price and guest capacity.
Paris has 54 invalid listings with zero price and zero guest capacity. 

. Sydney has no such invalid listings.
After removing invalid listings, Sydney has 33,630 valid listings. 34 listings are missing host_since, while all have valid price and guest capacity.

. After removing invalid listings, Rio has 26,608 valid listings. 24 of them are missing host_since information, but all have valid price and guest capacity.
Rio has 7 invalid listings with zero price and zero guest capacity.

#### 2. Prepare the data (of the three cities) for visualization:

#### . Creates a listing tables of neighbourhood, which groups each cities with their "neighbourhood" and calculate the mean price for each neighbourhood, sorted from lowest to highest average price.

Note: Euro as the baseline currency of comparison, but all the price are in local currency, thus prices will be convert to Euro.

##### Paris Neighbourhood Listings:
<img width="269" height="318" alt="image" src="https://github.com/user-attachments/assets/aa023546-f5f1-4372-b103-9ee447ae4da1" />

. Lowest mean price is Menilmontant with roughly 74 Euro, compare to the second lowest neighbours being Buttes-Chaumont, with only 8 Europ more.

<img width="252" height="277" alt="image" src="https://github.com/user-attachments/assets/c34c8c0d-fdab-443d-a64d-d04a764b741d" />

. Compare to Elysee which is a very luxurious neighbourhood in Paris, with a mean price average of 210 euro, but it's also sighnificantly more than the second most highest price neighbourhood being Louvre, which is 175 euro, a 35 euro different. 

##### Sydney Neighbourhood Listings:
<img width="233" height="271" alt="image" src="https://github.com/user-attachments/assets/b39f5c84-55e1-4fc6-a911-c538440a244c" />
<img width="280" height="309" alt="image" src="https://github.com/user-attachments/assets/4c3bb6a0-1a71-4025-9954-1269044278c6" />

. Lowest mean price in Sydney is the neighbourhood of Blacktown	with 93 AUD which is 55 Euro, compare to Burwood with the mean price of 95 AUD and 56 Euro.

. Meanwhile the most expensive neighbourhood in Sydney is Pittwater	with a massive 615 AUD or 363 Euro as it's mean price, and that is around 100+ Euro more than Mosman	at 432 AUD to 255 Euro.

#### Rio Dejaneiro Neighbourhood Listings:
<img width="251" height="332" alt="image" src="https://github.com/user-attachments/assets/41b59b24-35c8-4afc-ad2b-ff43d1e78aef" />
<img width="264" height="315" alt="image" src="https://github.com/user-attachments/assets/8c419f7f-7a6f-47ac-b36d-997e34d6c97c" />

. In Rio, the lowest mean price belong to the Vila Kosmos neighbourhood at 39 Brazilian Real which is roughly 6.3 Euro, and the highest mean price is 8120 Real, which is around 1k Euro, which is understandable because Brazil for the longest time have a big inequality between it's wealthier citizens and it's working population.

#### . Create a listing tables of accomodations, which filtered down to the most expensive neighborhood in Paris, grouped by the 'accommodations' columns and contain the mean price for each value of 'accommodates' sorted from lowest to highest average price.

<img width="389" height="196" alt="image" src="https://github.com/user-attachments/assets/ba40127d-cfa5-423b-aa60-55f91d70cdb9" />

. The basic coded structure to creates the accommodate listing is the following, query neighbourhood were choosen to have a similar values to each other using value count.

<img width="288" height="314" alt="image" src="https://github.com/user-attachments/assets/20e3de1f-1564-4ed2-a21c-b4c98fa35d56" />
<img width="247" height="264" alt="image" src="https://github.com/user-attachments/assets/b4d62734-29b7-4c07-9b3e-f151930475a4" />


. The cheapest listing by accomodations in Paris is, 0, with the price of 0, which just mean it's does not house any one.
. While the high accomdodations rentals values have higher prices

#### . Create a listing tables of over_time, which is grouped by the years of host_since column, and calculate a count of rows, representing the total number of new host and average price each years.



# Skills Utilized:
<br>

# Conclusion:
<br>
