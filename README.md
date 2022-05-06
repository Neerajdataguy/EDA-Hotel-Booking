# Hotel Booking Exploratory Data Analysis

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
