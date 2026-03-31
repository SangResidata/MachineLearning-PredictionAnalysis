Predicting airline ticket fares involves analyzing historical data, seasonality, and demand using machine learning to identify the best time to buy. Fares typically rise closer to departure, making 1–3 months out optimal for domestic flights (or 2–6 months for international). Prices are lowest on Tuesdays/Wednesdays and rise in weekly cycles as seats fill.  

Key Factors Influencing Price Predictions
    -  Time to Departure: Fares often increase 21, 14, and 7 days before the flight.
    -  Seat Availability: Higher demand equals higher prices.
    -  Seasonality/Holidays: High travel times spike prices.
    -  Time of Day: Early morning/late night flights are sometimes cheaper.  

    How to Predict and Save
    -  Use Prediction Tools: Utilize tools like Google Flights or the KAYAK Price Forecast to track trends.
    -  Set Price Alerts: Use services like Skyscanner or AirTrack to get alerts for price drops.
    -  Book Mid-Week: Late Tuesday or early Wednesday is often best for booking.
    -  Be Flexible: Adjusting travel dates can unlock significant savings. 

Predictive Modeling Techniques  

Modern systems use Machine Learning algorithms (like Linear Regression) and historical data to forecast trends. These models analyze factors like competitor pricing and special events (festivals, concerts) to estimate if a fare will rise or drop.

Research Questions

The aim of our study is to answer the below research questions:
a) Does price vary with Airlines?
b) How is the price affected when tickets are bought in just 1 or 2 days before departure?
c) Does ticket price change based on the departure time and arrival time?
d) How the price changes with change in Source and Destination?
e) How does the ticket price vary between Economy and Business class?  

DATA COLLECTION AND METHODOLOGY

Octoparse scraping tool was used to extract data from the website. Data was collected in two parts: one for economy class tickets and another for business class tickets. A total of 300261 distinct flight booking options was extracted from the site. Data was collected for 50 days, from February 11th to March 31st, 2022.
Data source was secondary data and was collected from Ease my trip website.  

DATASET

Dataset contains information about flight booking options from the website Easemytrip for flight travel between India's top 6 metro cities. There are 300261 datapoints and 11 features in the cleaned dataset.  

FEATURES

The various features of the cleaned dataset are explained below:
1) Airline: The name of the airline company is stored in the airline column. It is a categorical feature having 6 different airlines.
2) Flight: Flight stores information regarding the plane's flight code. It is a categorical feature.
3) Source City: City from which the flight takes off. It is a categorical feature having 6 unique cities.
4) Departure Time: This is a derived categorical feature obtained created by grouping time periods into bins. It stores information about the departure time and have 6 unique time labels.
5) Stops: A categorical feature with 3 distinct values that stores the number of stops between the source and destination cities.
6) Arrival Time: This is a derived categorical feature created by grouping time intervals into bins. It has six distinct time labels and keeps information about the arrival time.
7) Destination City: City where the flight will land. It is a categorical feature having 6 unique cities.
8) Class: A categorical feature that contains information on seat class; it has two distinct values: Business and Economy.
9) Duration: A continuous feature that displays the overall amount of time it takes to travel between cities in hours.
10)Days Left: This is a derived characteristic that is calculated by subtracting the trip date by the booking date.
11) Price: Target variable stores information of the ticket price.
