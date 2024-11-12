All the files are created using below Data. This file contains all the meta information regarding the columns described in the CSV files. we have provided 5 CSV files:

dim_date
dim_hotels
dim_rooms
fact_aggregated_bookings
fact_bookings
Column Description for dim_date:

date: This column represents the dates present in May, June and July.
mmm yy: This column represents the date in the format of mmm yy (monthname year).
week no: This column represents the unique week number for that particular date.
day_type: This column represents whether the given day is Weekend or Weekeday.
Column Description for dim_hotels:

property_id: This column represents the Unique ID for each of the hotels
property_name: This column represents the name of each hotel.
category: This column determines which class[Luxury, Business] a particular hotel/property belongs to.
city: This column represents where the particular hotel/property resides in.
Column Description for dim_rooms:

room_id: This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.
room_class: This column represents to which class[Standard, Elite, Premium, Presidential] particular room type belongs.
Column Description for fact_aggregated_bookings:

property_id: This column represents the Unique ID for each of the hotels.
check_in_date: This column represents all the check_in_dates of the customers.
room_category: This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.
successful_bookings: This column represents all the successful room bookings that happen for a particular room type in that hotel on that particular date.
capacity: This column represents the maximum count of rooms available for a particular room type in that hotel on that particular date.
Column Description for fact_bookings:

booking_id: This column represents the Unique Booking ID for each customer when they booked their rooms.
property_id: This column represents the Unique ID for each of the hotels
booking_date: This column represents the date on which the customer booked their rooms.
check_in_date: This column represents the date on which the customer check-in(entered) at the hotel.
check_out_date: This column represents the date on which the customer check-out(left) of the hotel.
no_guests: This column represents the number of guests who stayed in a particular room in that hotel.
room_category: This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.
booking_platform: This column represents in which way the customer booked his room.
ratings_given: This column represents the ratings given by the customer for hotel services.
booking_status: This column represents whether the customer cancelled his booking[Cancelled], successfully stayed in the hotel[Checked Out] or booked his room but not stayed in the hotel[No show].
revenue_generated: This column represents the amount of money generated by the hotel from a particular customer.
revenue_realized: This column represents the final amount of money that goes to the hotel based on booking status. If the booking status is cancelled, then 40% of the revenue generated is deducted and the
remaining is refunded to the customer. If the booking status is Checked Out/No show, then full revenue generated will goes to hotels.
