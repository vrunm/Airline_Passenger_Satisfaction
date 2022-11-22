# Airline_Passenger_Satisfaction
This dataset contains an airline passenger satisfaction survey. What factors are highly correlated to a satisfied (or dissatisfied) passenger
Gender: Gender of the passengers (Female, Male)
Customer Type: The customer type (Loyal customer, disloyal customer)



There is the following information about the passengers of some airline:

    Gender: male or female
    Customer type: regular or non-regular airline customer
    Age: the actual age of the passenger
    Type of travel: the purpose of the passenger's flight (personal or business travel)
    Class: business, economy, economy plus
    Flight distance
    Inflight wifi service: satisfaction level with Wi-Fi service on board (0: not rated; 1-5)
    Departure/Arrival time convenient: departure/arrival time satisfaction level (0: not rated; 1-5)
    Ease of Online booking: online booking satisfaction rate (0: not rated; 1-5)
    Gate location: level of satisfaction with the gate location (0: not rated; 1-5)
    Food and drink: food and drink satisfaction level (0: not rated; 1-5)
    Online boarding: satisfaction level with online boarding (0: not rated; 1-5)
    Seat comfort: seat satisfaction level (0: not rated; 1-5)
    Inflight entertainment: satisfaction with inflight entertainment (0: not rated; 1-5)
    On-board service: level of satisfaction with on-board service (0: not rated; 1-5)
    Leg room service: level of satisfaction with leg room service (0: not rated; 1-5)
    Baggage handling: level of satisfaction with baggage handling (0: not rated; 1-5)
    Checkin service: level of satisfaction with checkin service (0: not rated; 1-5)
    Inflight service: level of satisfaction with inflight service (0: not rated; 1-5)
    Cleanliness: level of satisfaction with cleanliness (0: not rated; 1-5)
    Departure delay in minutes
    Arrival delay in minutes

This data set contains a survey on air passenger satisfaction. The following classification problem is set:

It is necessary to predict which of the two levels of satisfaction with the airline the passenger belongs to:

    Satisfaction
    Neutral or dissatisfied


Conclusions after EDA:
1)The vast majority of the airline's customers are repeat customers.
2)Most of our clients flew for business rather than personal reasons.
3)About half of the passengers were in business class.
4)More than 60% of passengers were satisfied with the luggage transportation service (rating 4-5 out of 5).
5)More than 50% of passengers were comfortable sitting in their seats (rated 4-5 out of 5).
6)There was a strong correlation (96%) between the features 'Departure delay in minutes' and 'Arrival delay in minutes' to thier flight satisfaction. 
7)Most of the airline's regular customers are between the ages of 30 and 50 . 
The age range for non-regular customers is slightly smaller (from 25 to 40 years old, with an average of slightly less than 30).
Customers whose flight distance is long tend to fly in business class.

8)The more distance an airplane passenger travels (respectively, the longer they are in flight), the more satisfied they are with in-flight entertainment and extra legroom (on average).

9)Most of the passengers who flew in Economy Plus or Economy Class were dissatisfied with the flight, and those who were in Business Class were satisfied.
10)Almost all passengers who rated the wifi service 5 out of 5 were satisfied with the flight.
11)The majority of passengers who rated the comfort of the seats and the extra legroom at 4 and 5 points out of 5 were satisfied with the flight. 


After fitting several classification models it can be seen that the RandomForestClassifier performs the best:
DecisonTreeClassifier accuracy score: 94.2%
RandomForestClassifier accuracy score: 95.7%
LogisticRegression accuracy score: 81.9%
KNeighborsClassifieraccuracy score: 78.4%
