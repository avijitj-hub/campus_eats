# Campus Eats

### Introduction
This is the final project for the course ITCS 6160 Database Systems. This project is developed by Avijit Jaiswal. It is based on the Campus Eats system. This database management system provides an optimum solution for a campus delivery database, complete with a rating system. 

### Description
Food delivery services are very popular these days. The likes of Uber Eats and GrubHub immediately come to mind. **Campus Eats** is a campus controlled food delivery service catering to students, staff and faculty of a university campus. Such a delivery service requires a well-maintained database system. This database contains a large amount of data on Students, staff, restaurants, ratings, orders etc. It has certain pre-defined business rules. This database is based on work by Team Mavericks consisting of Dhananjay Arora, Akshay Babu, Sumit Kawale and Prashant Madaan in an earlier semester and is being used with permission. The database has been developed using SQL. MySQL Workbench has been used for designing the system. SQL queries are used to design and populate the database. Stored procedures are written to calculate maximum, minimum and average ratings. Advanced queries are used to generate insights from the data. EER Diagram is designed to analyze the structure of the database. Use case diagram is designed to view the applications of the rating system.

### Business Rules
1. Ratings will be given on a scale of 1 to 5.
1. Only students can be drivers.
1. There is one overall rating, one restaurant rating and one delivery rating.
1. Generally, ratings are associated with individual orders.
1. However, not every order is supposed to have a rating.
1. Some orders may have just a restaurant rating or just a delivery rating.
1. A restaurant rating may further have a food rating and a price rating.

### Extended Entity Relationship Diagram (EERD)
<br></br>
<img src="https://github.com/avijitj-hub/campus_eats/blob/main/images/EERD%20Campus%20Eats.PNG" />
<br></br>
EER is a high-level data model that incorporates the extensions to the original ER model. Enhanced ERD are high level models that represent the requirements and complexities of complex database. The Campus Eats database design represents interactions between various entities. Students and staff can place orders. Orders are received by the restaurants. Customers can provide ratings. Drivers and restaurants can receive ratings. Vehicles can be present at different locations. I have added a rating system to the original database. The tables ratings, driver_rating and restaurant_rating have been added to create a holistic rating model. In this way, every order is associated with a driver, restaurant and customer. Every rating is associated with an order and a driver or restaurant. We can easily find the records associated with every driver, restaurant or vehicle. This EER diagram was generated by reverse-engineering the database using MySQL Workbench. It lucidly illustrates the relationships between the various components of the system.

### Use Case Diagram
<img src="https://github.com/avijitj-hub/campus_eats/blob/main/images/use_case_diagram.jpg" height="50%" width="60%" />

This diagram depicts the various applicable use cases for different actors in the system. It is derived from the business rules and application capabilities of the system. A use case diagram is a graphical depiction of a user's possible interactions with a system. A use case diagram shows various use cases and different types of users the system has. There are four main Actors in the system namely Drivers, Restaurants, Customers and Administrators. Customers can create new orders. They can also provide ratings for drivers and restaurants. Drivers can receive new delivery orders. Each driver has an associated vehicle. Only students can be drivers. Drivers can receive punctual and politeness ratings. Restaurants can receive new orders from customers. Restaurants can assign deliveries to drivers. Restaurants can receive ratings based on the quality and price of food. Administrators can view driver and restaurant ratings. They can check order delivery status. They can ensure that the entire system is running smoothly.  
<br></br>

### Data Dictionary

View the complete [Data Dictionary] (https://github.com/avijitj-hub/campus_eats/blob/main/data_dictionary.md) here.

### Stored Procedures
#### #1 Driver MaxMinAvg
<img src="https://github.com/avijitj-hub/campus_eats/blob/main/images/sp_driver.jpg" height="45%" width="45%" />
The first stored procedure is used to calculate the maximum, minimum  and average rating of each driver. It can be very useful to find out which drivers are being liked the most by customers and so forth. It can also be used to determine if any drivers are required to undergo disciplinary action. This function calculates the maximum, minimum and average ratings using methods and categorizes them according to unique driver_id.
<br></br>

#### #2 Restaurant MaxMinAvg
<img src="https://github.com/avijitj-hub/campus_eats/blob/main/images/sp_restaurant.jpg" height="40%" width="45%" />
The second stored procedure is used to calculate the maximum, minimum and average rating for each restaurant. Again, it can be very useful to system users to find out which restaurants are performing the best and which ones not so much. These insights can be used to determine the overall performance of restaurants. Restaurants can use it to find out where they stand with respect to their competition. This function determines the maximum, minimum and average ratings using methods and assigns them according to each restaurant's unique restaurant_id.
<br></br>

### Advanced Queries
#### #1 Top-rated Cars
<img src="https://github.com/avijitj-hub/campus_eats/blob/main/images/advq1.jpg" height="50%" width="50%"/>
The first advanced query is used to determine which cars are preferred by the top-rated drivers. This can be useful to analyze if highly-rated drivers prefer to use cars of any particular makes. We have written an advanced query in SQL which employs both a nested SELECT and a sub-query as well as a condition using WHERE. To put the result together we have used a JOIN statement and finally sorted the end result in descending order.
<br></br>

#### #2 Highest-revenue Restaurants
<img src="https://github.com/avijitj-hub/campus_eats/blob/main/images/advq2.jpg" height="60%" width="60%"/>
The second advanced query is used to show ratings of the restaurants that are generating the highest revenue. It can be interesting to find out how the restaurants attracting the most business are being rated by their customers. Also, it would be interesting to see if there are any small restaurants with a small user base that are rated highly by their customers. In this query we have used an aggregation function namely SUM, after employing GROUP BY command. We have again merged two different tables using JOIN statement to yield interesting insights on the data.
