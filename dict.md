# Schema Report for database: campus_eats_jaiswal

<a id="home">Table List</a>  

*   [delivery](#delivery)
*   [driver](#driver)
*   [driver_rating](#driver_rating)
*   [faculty](#faculty)
*   [location](#location)
*   [orders](#orders)
*   [person](#person)
*   [ratings](#ratings)
*   [restaurant](#restaurant)
*   [restaurant_audit](#restaurant_audit)
*   [restaurant_rating](#restaurant_rating)
*   [staff](#staff)
*   [student](#student)
*   [vehicle](#vehicle)

<a id="delivery"></a>

<table style="width:100%"><caption>Table: delivery</caption>

<tbody>

<tr>

<td>Table Comments</td>

<td colspan="6"></td>

</tr>

<tr>

<td colspan="7">Columns</td>

</tr>

<tr>

<th>Name</th>

<th>Data Type</th>

<th>Nullable</th>

<th>PK</th>

<th>FK</th>

<th>Default</th>

<th>Comment</th>

</tr>

<tr>

<td>delivery_id</td>

<td>INT</td>

<td>Yes</td>

<td>Yes</td>

<td>No</td>

<td></td>

<td></td>

</tr>

<tr>

<td>driver_id</td>

<td>INT</td>

<td>Yes</td>

<td>No</td>

<td>Yes</td>

<td></td>

<td></td>

</tr>

<tr>

<td>vehicle_id</td>

<td>INT</td>

<td>Yes</td>

<td>No</td>

<td>Yes</td>

<td></td>

<td></td>

</tr>

<tr>

<td>delivery_time</td>

<td>DATETIME</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

</tbody>

</table>

[Table List](#home)  
<a id="driver"></a>

<table style="width:100%"><caption>Table: driver</caption>

<tbody>

<tr>

<td>Table Comments</td>

<td colspan="6"></td>

</tr>

<tr>

<td colspan="7">Columns</td>

</tr>

<tr>

<th>Name</th>

<th>Data Type</th>

<th>Nullable</th>

<th>PK</th>

<th>FK</th>

<th>Default</th>

<th>Comment</th>

</tr>

<tr>

<td>driver_id</td>

<td>INT</td>

<td>Yes</td>

<td>Yes</td>

<td>No</td>

<td></td>

<td></td>

</tr>

<tr>

<td>student_id</td>

<td>INT</td>

<td>Yes</td>

<td>No</td>

<td>Yes</td>

<td></td>

<td></td>

</tr>

<tr>

<td>license_number</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>date_hired</td>

<td>DATE</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>rating</td>

<td>FLOAT</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

</tbody>

</table>

[Table List](#home)  
<a id="driver_rating"></a>

<table style="width:100%"><caption>Table: driver_rating</caption>

<tbody>

<tr>

<td>Table Comments</td>

<td colspan="6"></td>

</tr>

<tr>

<td colspan="7">Columns</td>

</tr>

<tr>

<th>Name</th>

<th>Data Type</th>

<th>Nullable</th>

<th>PK</th>

<th>FK</th>

<th>Default</th>

<th>Comment</th>

</tr>

<tr>

<td>rating_id</td>

<td>INT</td>

<td>Yes</td>

<td>Yes</td>

<td>No</td>

<td></td>

<td></td>

</tr>

<tr>

<td>punctual_rating</td>

<td>INT</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>polite_rating</td>

<td>INT</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>driver_id</td>

<td>INT</td>

<td>Yes</td>

<td>No</td>

<td>Yes</td>

<td></td>

<td></td>

</tr>

<tr>

<td>order_id</td>

<td>INT</td>

<td>Yes</td>

<td>No</td>

<td>Yes</td>

<td></td>

<td></td>

</tr>

<tr>

<td>hybrid_driver_rating</td>

<td>DOUBLE</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

</tbody>

</table>

[Table List](#home)  
<a id="faculty"></a>

<table style="width:100%"><caption>Table: faculty</caption>

<tbody>

<tr>

<td>Table Comments</td>

<td colspan="6"></td>

</tr>

<tr>

<td colspan="7">Columns</td>

</tr>

<tr>

<th>Name</th>

<th>Data Type</th>

<th>Nullable</th>

<th>PK</th>

<th>FK</th>

<th>Default</th>

<th>Comment</th>

</tr>

<tr>

<td>faculty_id</td>

<td>INT</td>

<td>Yes</td>

<td>Yes</td>

<td>No</td>

<td></td>

<td></td>

</tr>

<tr>

<td>person_id</td>

<td>INT</td>

<td>Yes</td>

<td>No</td>

<td>Yes</td>

<td></td>

<td></td>

</tr>

<tr>

<td>title</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>degree_college</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>highest_degree</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

</tbody>

</table>

[Table List](#home)  
<a id="location"></a>

<table style="width:100%"><caption>Table: location</caption>

<tbody>

<tr>

<td>Table Comments</td>

<td colspan="6"></td>

</tr>

<tr>

<td colspan="7">Columns</td>

</tr>

<tr>

<th>Name</th>

<th>Data Type</th>

<th>Nullable</th>

<th>PK</th>

<th>FK</th>

<th>Default</th>

<th>Comment</th>

</tr>

<tr>

<td>location_id</td>

<td>INT</td>

<td>Yes</td>

<td>Yes</td>

<td>No</td>

<td></td>

<td></td>

</tr>

<tr>

<td>location_name</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>location_address</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>latitude</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>longitude</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>drop_off_point</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

</tbody>

</table>

[Table List](#home)  
<a id="orders"></a>

<table style="width:100%"><caption>Table: orders</caption>

<tbody>

<tr>

<td>Table Comments</td>

<td colspan="6"></td>

</tr>

<tr>

<td colspan="7">Columns</td>

</tr>

<tr>

<th>Name</th>

<th>Data Type</th>

<th>Nullable</th>

<th>PK</th>

<th>FK</th>

<th>Default</th>

<th>Comment</th>

</tr>

<tr>

<td>order_id</td>

<td>INT</td>

<td>Yes</td>

<td>Yes</td>

<td>No</td>

<td></td>

<td></td>

</tr>

<tr>

<td>person_id</td>

<td>INT</td>

<td>Yes</td>

<td>No</td>

<td>Yes</td>

<td></td>

<td></td>

</tr>

<tr>

<td>delivery_id</td>

<td>INT</td>

<td>Yes</td>

<td>No</td>

<td>Yes</td>

<td></td>

<td></td>

</tr>

<tr>

<td>location_id</td>

<td>INT</td>

<td>Yes</td>

<td>No</td>

<td>Yes</td>

<td></td>

<td></td>

</tr>

<tr>

<td>driver_id</td>

<td>INT</td>

<td>Yes</td>

<td>No</td>

<td>Yes</td>

<td></td>

<td></td>

</tr>

<tr>

<td>restaurant_id</td>

<td>INT</td>

<td>Yes</td>

<td>No</td>

<td>Yes</td>

<td></td>

<td></td>

</tr>

<tr>

<td>total_price</td>

<td>FLOAT</td>

<td>Yes</td>

<td>No</td>

<td>No</td>

<td></td>

<td></td>

</tr>

<tr>

<td>delivery_charge</td>

<td>FLOAT</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

</tbody>

</table>

[Table List](#home)  
<a id="person"></a>

<table style="width:100%"><caption>Table: person</caption>

<tbody>

<tr>

<td>Table Comments</td>

<td colspan="6"></td>

</tr>

<tr>

<td colspan="7">Columns</td>

</tr>

<tr>

<th>Name</th>

<th>Data Type</th>

<th>Nullable</th>

<th>PK</th>

<th>FK</th>

<th>Default</th>

<th>Comment</th>

</tr>

<tr>

<td>person_id</td>

<td>INT</td>

<td>Yes</td>

<td>Yes</td>

<td>No</td>

<td></td>

<td></td>

</tr>

<tr>

<td>person_name</td>

<td>VARCHAR(300)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>person_email</td>

<td>VARCHAR(150)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>cell</td>

<td>BIGINT</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

</tbody>

</table>

[Table List](#home)  
<a id="ratings"></a>

<table style="width:100%"><caption>Table: ratings</caption>

<tbody>

<tr>

<td>Table Comments</td>

<td colspan="6"></td>

</tr>

<tr>

<td colspan="7">Columns</td>

</tr>

<tr>

<th>Name</th>

<th>Data Type</th>

<th>Nullable</th>

<th>PK</th>

<th>FK</th>

<th>Default</th>

<th>Comment</th>

</tr>

<tr>

<td>rating_id</td>

<td>INT</td>

<td>Yes</td>

<td>Yes</td>

<td>No</td>

<td></td>

<td></td>

</tr>

<tr>

<td>general_rating</td>

<td>INT</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>order_id</td>

<td>INT</td>

<td>Yes</td>

<td>No</td>

<td>Yes</td>

<td></td>

<td></td>

</tr>

</tbody>

</table>

[Table List](#home)  
<a id="restaurant"></a>

<table style="width:100%"><caption>Table: restaurant</caption>

<tbody>

<tr>

<td>Table Comments</td>

<td colspan="6"></td>

</tr>

<tr>

<td colspan="7">Columns</td>

</tr>

<tr>

<th>Name</th>

<th>Data Type</th>

<th>Nullable</th>

<th>PK</th>

<th>FK</th>

<th>Default</th>

<th>Comment</th>

</tr>

<tr>

<td>restaurant_id</td>

<td>INT</td>

<td>Yes</td>

<td>Yes</td>

<td>No</td>

<td></td>

<td></td>

</tr>

<tr>

<td>location</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>restaurant_name</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>schedule</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>website</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>restaurant_rating</td>

<td>FLOAT</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

</tbody>

</table>

[Table List](#home)  
<a id="restaurant_audit"></a>

<table style="width:100%"><caption>Table: restaurant_audit</caption>

<tbody>

<tr>

<td>Table Comments</td>

<td colspan="6"></td>

</tr>

<tr>

<td colspan="7">Columns</td>

</tr>

<tr>

<th>Name</th>

<th>Data Type</th>

<th>Nullable</th>

<th>PK</th>

<th>FK</th>

<th>Default</th>

<th>Comment</th>

</tr>

<tr>

<td>audit_id</td>

<td>INT</td>

<td>Yes</td>

<td>Yes</td>

<td>No</td>

<td></td>

<td></td>

</tr>

<tr>

<td>restaurant_id</td>

<td>INT</td>

<td>Yes</td>

<td>No</td>

<td>No</td>

<td></td>

<td></td>

</tr>

<tr>

<td>location</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>restaurant_name</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>type_of_change</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>date_of_change</td>

<td>DATETIME</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

</tbody>

</table>

[Table List](#home)  
<a id="restaurant_rating"></a>

<table style="width:100%"><caption>Table: restaurant_rating</caption>

<tbody>

<tr>

<td>Table Comments</td>

<td colspan="6"></td>

</tr>

<tr>

<td colspan="7">Columns</td>

</tr>

<tr>

<th>Name</th>

<th>Data Type</th>

<th>Nullable</th>

<th>PK</th>

<th>FK</th>

<th>Default</th>

<th>Comment</th>

</tr>

<tr>

<td>rating_id</td>

<td>INT</td>

<td>Yes</td>

<td>Yes</td>

<td>No</td>

<td></td>

<td></td>

</tr>

<tr>

<td>food_rating</td>

<td>INT</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>cost_rating</td>

<td>INT</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>restaurant_id</td>

<td>INT</td>

<td>Yes</td>

<td>No</td>

<td>Yes</td>

<td></td>

<td></td>

</tr>

<tr>

<td>order_id</td>

<td>INT</td>

<td>Yes</td>

<td>No</td>

<td>Yes</td>

<td></td>

<td></td>

</tr>

<tr>

<td>hybrid_restaurant_rating</td>

<td>DOUBLE</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

</tbody>

</table>

[Table List](#home)  
<a id="staff"></a>

<table style="width:100%"><caption>Table: staff</caption>

<tbody>

<tr>

<td>Table Comments</td>

<td colspan="6"></td>

</tr>

<tr>

<td colspan="7">Columns</td>

</tr>

<tr>

<th>Name</th>

<th>Data Type</th>

<th>Nullable</th>

<th>PK</th>

<th>FK</th>

<th>Default</th>

<th>Comment</th>

</tr>

<tr>

<td>staff_id</td>

<td>INT</td>

<td>Yes</td>

<td>Yes</td>

<td>No</td>

<td></td>

<td></td>

</tr>

<tr>

<td>person_id</td>

<td>INT</td>

<td>No</td>

<td>No</td>

<td>Yes</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>position</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>is_admin</td>

<td>VARCHAR(1)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>'N'</td>

<td></td>

</tr>

</tbody>

</table>

[Table List](#home)  
<a id="student"></a>

<table style="width:100%"><caption>Table: student</caption>

<tbody>

<tr>

<td>Table Comments</td>

<td colspan="6"></td>

</tr>

<tr>

<td colspan="7">Columns</td>

</tr>

<tr>

<th>Name</th>

<th>Data Type</th>

<th>Nullable</th>

<th>PK</th>

<th>FK</th>

<th>Default</th>

<th>Comment</th>

</tr>

<tr>

<td>student_id</td>

<td>INT</td>

<td>Yes</td>

<td>Yes</td>

<td>No</td>

<td></td>

<td></td>

</tr>

<tr>

<td>person_id</td>

<td>INT</td>

<td>Yes</td>

<td>No</td>

<td>Yes</td>

<td></td>

<td></td>

</tr>

<tr>

<td>graduation_year</td>

<td>INT</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>major</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>type</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

</tbody>

</table>

[Table List](#home)  
<a id="vehicle"></a>

<table style="width:100%"><caption>Table: vehicle</caption>

<tbody>

<tr>

<td>Table Comments</td>

<td colspan="6"></td>

</tr>

<tr>

<td colspan="7">Columns</td>

</tr>

<tr>

<th>Name</th>

<th>Data Type</th>

<th>Nullable</th>

<th>PK</th>

<th>FK</th>

<th>Default</th>

<th>Comment</th>

</tr>

<tr>

<td>vehicle_id</td>

<td>INT</td>

<td>Yes</td>

<td>Yes</td>

<td>No</td>

<td></td>

<td></td>

</tr>

<tr>

<td>vehicle_plate</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>model</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

<tr>

<td>make</td>

<td>VARCHAR(75)</td>

<td>No</td>

<td>No</td>

<td>No</td>

<td>NULL</td>

<td></td>

</tr>

</tbody>

</table>

[Table List](#home)
