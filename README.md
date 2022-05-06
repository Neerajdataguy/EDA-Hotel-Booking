# Hotel Bookings Exploratory Data Analysis

## Objective
We are provided with a hotel bookings dataset. 

Out main objective is perform EDA on the given dataset and draw useful conclusions about general trends in hotel bookings and how factors governing hotel bookings interact with each other.

## Dataset
We are given a hotel bookings dataset. This dataset contains booking information for a city hotel and a resort hotel. It contains the following features.

```
- hotel: Name of hotel ( City or Resort)
- is_canceled: Whether booking is cancelled or not (0 for no cancelled and 1 for cancelled)
- lead_time: time (in days) between booking transaction and actual arrival.
- arrival_date_year: Year of arrival
- arrival_date_month: month of arrival
- arrival_date_week_number: week number of arrival date.
- arrival_date_day_of_month: Day of month of arrival date
- stays_in_weekend_nights: No. of weekend nights spent in hotel
- stays_in_week_nights: : No. of week nights spent in hotel
- adults: No. of adults in single booking record.
- children: No. of children in single booking record.
- babies: No. of babies in single booking record. 
- meal: Type of meal chosen 
- country: Country of origin of customers (as mentioned by them)
- market_segment: What segment via booking was made and for what purpose.
- distribution_channel: Via which medium booking was made.
- is_repeated_guest: Whether the customer has made any booking before(0 for No and 1 for 
                     Yes)
- previous_cancellations: No. of previous cancelled bookings.
- previous_bookings_not_canceled: No. of previous non-cancelled bookings.
- reserved_room_type: Room type reserved by customer.
- assigned_room_type: Room type assigned to customer.
- booking_changes: No. of booking changes done by customers
- deposit_type: Type of deposit at time of making booking (No deposit/ Refundable/ No refund)
- agent: Id of agent for booking
- company: Id of company making booking
- days_in_waiting_list: No. of days in waiting list.
- customer_type: Type of customer(Transient, Group, etc.)
- adr: Average Daily rate.
- required_car_parking_spaces: No. of car parking asked in booking
- total_of_special_requests: total no. of special request.
- reservation_status: Whether customer has checked out or cancelled,or not showed 
- reservation_status_date: Date of making reservation status.
```

- Total number of rows in data : 119390
- Total number of columns : 32
## Data Cleaning and Feature Engineering

### (1) Removing Duplicate rows
All duplicate rows were dropped..

### (2) Handling null values
- Null values in columns `company` and `agent` were replaced by 0.
- Null values in column `country` were replaced by 'others'.
- Null values in column `children` were replaced by mean of the column.
  

### (3) Converting columns to appropriate data types

- Changed datatype of `children`, `company`, `agent` to int type.
- Changed datatype of `reservation_status_date` to date type.

### (4) Removing outliers

- One outlier was found in `adr` column. Simply dropped it.

### (5) Creating new columns
- Created new column `total_stay` by adding `stays_in_weekend_nights`+`stays_in_week_nights`.
- Created new column `total_people` by adding `adults`+`children`+`babies`.

## Exploratory Data Analysis

Mainly performed using Matplotlib and Seaborn library and the following graph and plots had been used:
  -  Bar Plot.
  -  Histogram.
   - Scatter Plot.
   - Pie Chart.
   - Line Plot.
   - Heatmap.
- Box Plot
             
###  Univariate Analysis:

We tried to answer following questions
```
 Q1) Which agent makes most no. of bookings?
 Q2) Which room type is in most demand and which room type generates highest adr?
 Q3) Which meal type is most preffered meal of customers?
 Q4) What is percentage of bookings in each hotel?
 Q5) Which is the most common channel for booking hotels?
 Q6) Which are the most busy months?
 Q7) Which agent makes most no. of bookings?
 Q8)From which country most of the guests are coming ?
 Q9) How long do people stay at the hotels?
```




### Bivariate Analysis :

We tried to answer following questions
```
Q1)  Which hotel seems to make more revenue?
Q2)  Which hotel has higher lead time?
Q3)  What is preferred stay length in each hotel?
Q4)  Which hotel has higher bookings cancellation rate.
Q5)  Which hotel has high chance that its customer will return for another stay?
Q6)  Which channel is mostly used for early booking of hotels?
Q7)  Which channel has longer average waiting time?
Q8)  Which distribution channel brings better revenue generating deals for hotels?
Q9)  Which significant distribution channel has highest cancellation percentage?
Q10) Does longer waiting period or longer lead time causes the cancellation of bookings?
Q11) Whether not getting allotted the same room type as demanded is the main cause of cancellation fo bookings?
Q12) Does not alloting same room as demanded affects adr ? 
Q13) What is the trend of bookings within a month?
Q14) Which types of customers mostly make bookings?
```

## Conclusion


