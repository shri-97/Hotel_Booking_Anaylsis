# Hotel_Booking_Anaylsis
# Objective:
I have Hotel Booking dataset.The main objective of this project is explore the given dataset and find useful conclusion about general trends in hotel booking and discover how these factors affect on hospitality business.
# Dataset:
The dataset have information of city and resort hotel. This dataset have 11390 rows and 32 coulumns. The columns from the dataset is as follows:

Hotel: Type of hotel(City or Resort)

is_cancelled: If the booking was cancelled(1) or not(0)

lead_time: Number of days before the actual arrival of the guests

arrival_date_year: Year of arrival date

arrival_date_month: Month of arrival date

arrival_date_week_number: Week number of year for arrival date

arrival_date_day_of_month: Day of arrival date

stays_in_weekend_nights: Number of weekend nights(Saturday or Sunday) spent at the hotel by the guests.

stays_in_weel_nights: Number of weeknights(Monday to Friday) spent at the hotel by the guests.

adults: Number of adults among the guests

children: Number of children

babies: Number of babies

meal: Type of meal booked

country: country of the guests

market_segment: Designation of market segment

distribution_channel: Name of booking distribution channel

is_repeated_guest: If the booking was from a repeated guest(1) or not(0)

previous_cancellation: Number of previous bookings that were cancelled by the customer prior to the current booking

previous_bookings_not_cancelled: Number of previous bookins not cancelled by the customer prior to the current booking

reserved_room_type: Code from room type reserved

assigned_room_type: Code of room type assigned

booking_changes: Number of changes made to the booking

deposit_type: Type of deposite made by the guest

agent: ID of travel agent who made the booking

comapny: ID of the company that made the booking

days_in_waiting_list: Number of the days the booking was in the waiting list

customer_type: Type of customer, assuming one of four categories

adr: Average daily rate

required_car_parking_spaces: Number of car parking spaces required bt the customer

total_of_special_requesrs: Number of special requests made by the customer

reservation_statuse: Reservation status(Canceled, check-out or no-show)

reservation_status_date: Date at which the last reservation status was updated

# Data cleaning and manipulation:

# Duplicate values

Dataset have 31994 duplicate values. so these duplicate values are removedfrom dataset using.drop_dupliactes(). After droping duplicate value shape of the dataset become 87396 rows and 32 columns.

# Missing values/null values
Given dataset have 4 columns company, aent, country and children missing values so these values are replace by usin .fillna() function.

# Addition of new columns
Total_people and Total_stay these two columns are added in given dataset Some rows are removed from columns adults, children and babies.

# Exploratory Data Analysis

The EDA is done by using 3 analysis Univariate, Bivariate and Multivariate analysis. For the datavisualization following charts are used:

Pie chart

Barplot

Countplot

lineplot

Kdeplot

Boxplot

# Performed EDA and tried answering the following questions:
1) Which type of hotel is mostly preferred by the guests?
2) Which type of food is mostly preferred by the guests?
3) Which room type is in most demand?
4) What is preferred stay length in each hotel?
5) Which year had a highest booking?
6) In Which month most of the bookings happened?
7) Which hotel has high chance that its customer will return for another stay?
8) Which hotel has higher lead time?
9) Which channel is mostly used for early booking of hotels?
10) How much average price for room per night?
11) Which agent made the most bookings?
12) Which distribution channel brings better revenue generating deals for hotels?
13) From which country the most guests are coming?
14) Which Hotel type has the highest ADR?
15) Waiting period effect on booking cancelation
16) Effect of changing the allocated room on Booking cancelation?
17) Checking the booking percentage on differnt typeof customer i.e single, couple and family/friends
18) Predicting whether or not a hotel was likely to receive a disproportionately high number of special requests?
19)What is the percentage distribution of required_car_parking_spaces? 

# Conclusion:

1.	City hotels are the most preferred hotel type by the guests. We can say City hotel is the busiest hotel.
2.	BB (Bed & Breakfast) is the most preferred type of meal by the guests.
3.	Most demanded room type is A.
4.	Most common stay length is less than 4 days and generally people prefer City hotel for short stay, but for long stays, Resort Hotel is preferred.
5.	Most of the bookings for City hotels and Resort hotel were happened in 2016.
6.	Most number of guests comes in month of August.
7.	Both hotels have very small percentage that customer will repeat, but Resort hotel has slightly higher repeat % than City Hotel.
8.	City hotel has slightly higher median lead time. Also median lead time is significantly higher in each case, this means customers generally plan their hotel visits way to early.
9.	Most of the bookings were made through TA/TO (travel agents/Tour operators)
10.	This figure shows the average price per room, depending on its type and the standard deviation. Note that due to data anonymization rooms with the same type letter may not necessarily be the same across hotels.
11.	The insight found here is Agent no. 9 made most of the bookings.
12.	GDS channel brings higher revenue generating deals for City hotel, in contrast to that most bookings come via TA/TO. City Hotel can work to increase outreach on GDS channels to get more higher revenue generating deals.
13.	Most guest are from Portugal and other European countries.
14.	Average ADR for city hotel is high as compared to resort hotels. These City hotels are generating more revenue than the resort hotels.
15.	We see that most of the bookings that are cancelled have waiting period of less 150 days but also most of bookings that are not cancelled also have waiting period less than 150 days. Hence this shows that waiting period has no effect on cancellation of bookings. \ \ Also, lead time has no affect on cancellation of bookings, as both curves of cancelation and not cancelation are similar for lead time too
16.	We see that not getting same room as demanded is not the case of cancellation of rooms. A significant percentage of bookings are not cancelled even after getting different room as demanded
17.	Mostly bookings are done by couples(although we are not sure that they are couple as data doesn't tell about that)
18.	It is clear from graph that their is a sudden surge in arrival no of couples and family in months of July and August. So better plans can be planned accordingly at that time for these type of customers.
19.	All of market segment mostly have special request.91.6 % guests did not required the parking space. only 8.3 % guests required only 1 parking space.



