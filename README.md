# Ola Booking Data Analysis Project

## Project Overview

The Ola Booking Data Analysis project aims to analyze ride-sharing data to understand customer behavior, ride patterns, service performance, and driver efficiency. This project uses a PostgreSQL database to perform various SQL queries to uncover key insights and answer specific business questions related to customer behavior, ride efficiency, service performance, and driver quality.

## Objectives

The main objectives of this project are:
- To analyze the ride-sharing data for different booking patterns.
- To identify the peak hours, most popular vehicle types, and repeat customers.
- To examine the impact of payment methods and discounts on total booking values.
- To analyze ride cancellations and incomplete rides to understand reasons and patterns.
- To compute performance metrics such as ride completion rates, average ride distance, and driver performance.
- To generate reports to aid business decision-making processes for improving service efficiency.

## Database Setup

This project utilizes a PostgreSQL database with the following table structure for `ola_booking`:

### `ola_booking` Table Schema
| Column Name                | Data Type     |
|----------------------------|---------------|
| Date                        | DATE          |
| Time                        | TIME          |
| Booking_ID                  | VARCHAR(20)   |
| Booking_Status              | VARCHAR(25)   |
| Customer_ID                 | VARCHAR(25)   |
| Vehicle_Type                | VARCHAR(25)   |
| Pickup_Location             | VARCHAR(25)   |
| Drop_Location               | VARCHAR(25)   |
| V_TAT                       | VARCHAR(25)   |
| C_TAT                       | VARCHAR(25)   |
| Canceled_Rides_by_Customer  | VARCHAR(50)   |
| Canceled_Rides_by_Driver    | VARCHAR(40)   |
| Incomplete_Rides            | VARCHAR(25)   |
| Incomplete_Rides_Reason     | VARCHAR(25)   |
| Booking_Value               | BIGINT        |
| Payment_Method              | VARCHAR(25)   |
| Ride_Distance               | VARCHAR(25)   |
| Driver_Ratings              | VARCHAR(25)   |
| Customer_Rating             | VARCHAR(25)   |

### Sample Queries:
1. **Identify the top 3 peak booking hours based on ride volume.**
2. **Find the most common vehicle type booked by frequent customers.**
3. **Determine the percentage of repeat customers in the dataset.**
4. **Rank payment methods by their total booking value contribution.**
5. **Calculate the average customer rating for each vehicle type in different cities.**

## Findings

Through the analysis, the following findings were uncovered:
1. **Peak Booking Hours**: The top 3 peak hours for bookings were identified, helping to understand when the most rides are requested.
2. **Common Vehicle Type**: The most common vehicle types were identified based on frequent customer bookings, providing insights into customer preferences.
3. **Repeat Customer Percentage**: The percentage of repeat customers was calculated to understand customer loyalty.
4. **Revenue Contributions by Payment Methods**: The ranking of payment methods based on their contribution to total revenue helps understand which methods are preferred by customers.
5. **Ride Completion Rates**: Completion rates for different cities were computed, revealing areas with higher cancellation or incomplete ride rates.
6. **Cancellation and Incomplete Ride Reasons**: The most common reasons for cancellations and incomplete rides were identified, aiding in the improvement of customer satisfaction.

## Reports

The project generated several analytical reports that include:
- **Peak Booking Hour Analysis**: Insights into the busiest hours for ride-sharing services.
- **Vehicle Preference by Customer**: Identification of the most frequently used vehicle types and popular locations.
- **Cancellation Analysis**: Identifying reasons behind ride cancellations and the most canceled locations.
- **Revenue Analysis**: Total revenue by city, highlighting the most profitable locations.
- **Driver and Customer Rating**: Performance metrics on driver ratings and customer ratings across various vehicle types.

## Conclusion

This project provides actionable insights that can be used to improve ride-sharing operations:
- **Improve Customer Satisfaction**: By addressing the reasons for ride cancellations and incomplete rides, customer experience can be improved.
- **Optimize Resources**: Knowing peak booking hours helps in optimizing vehicle allocation.
- **Focus on High Revenue Locations**: Identifying cities with the highest revenue potential can aid in better resource management and targeted marketing.
- **Enhance Driver Performance**: By monitoring driver ratings, service quality can be maintained and improved.

This analysis is essential for Ola to optimize their ride-sharing services, increase customer satisfaction, and drive overall revenue growth.

---

### Built With
- **PostgreSQL**: Database used for querying and analysis.
- **SQL**: Language used to write the queries and perform the data analysis.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

