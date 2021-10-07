# Campus Eats

### INTRODUCTION
This is the final project for the course ITCS 6160 Database Systems. This project is developed by Avijit Jaiswal. It is based on the Campus Eats system. This database management system provides an optimum solution for a campus delivery database, complete with a rating system. 

### DESCRIPTION
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
<br>
<img src="https://github.com/avijitj-hub/campus_eats/blob/main/images/EERD%20Campus%20Eats.PNG" height="90%" width="90%" />
<br>   
### Use Case Diagram
<br>
<img src="https://github.com/avijitj-hub/campus_eats/blob/main/images/use_case_diagram.jpg" height="50%" width="60%" />
<br>
### Stored Procedures
<br>
<img src="https://github.com/avijitj-hub/campus_eats/blob/main/images/sp_driver.jpg" height="45%" width="45%" />
<br>
<img src="https://github.com/avijitj-hub/campus_eats/blob/main/images/sp_restaurant.jpg" height="40%" width="45%" />
<br>
### Advanced Queries
<br>
<img src="https://github.com/avijitj-hub/campus_eats/blob/main/images/advq1.jpg" height="50%" width="50%"/>
<br>
<img src="https://github.com/avijitj-hub/campus_eats/blob/main/images/advq2.jpg" height="60%" width="60%"/>
