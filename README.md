Download Link: https://assignmentchef.com/product/solved-contact-management-system-for-a-salon
<br>
Create a simple, user friendly contact management system for a salon. The application should be able to store all contacts who have visited the salon, the date visited, the services rendered and by whom. It should also be able to create flags to notify the user when they are due for a new appointment. This will enable the owner to maintain her records much more easily, allow for backups, and allow for much greater interaction with the data as desired than the current paper system.

<strong>Business Problem: </strong>

Salon owner is currently keeping all clients in an address book and needs a way to digitally keep track of the clients and the services and products they buy as well as time they should return.

<strong>Scope:</strong>

Recording client information, appointments, stylists, services and services rendered, products and products rendered are within the scope. It will also allow for querying client information. Keeping track of the inventory and managing scheduling is out of the scope.

<strong>Business Process Flow:</strong>

<ol>

 <li>A client enters or calls the salon.</li>

 <li>They schedule a service with a stylist.</li>

 <li>The service is performed by the stylist and they recommend a date to return.</li>

 <li>The client can purchase product(s) at any point during the process.</li>

</ol>

<strong>Data Elements Verification:</strong>

The following table shows all data elements identified in the user requirements and represented in the ER model.The verification column is based on the ER model.




<table width="624">

 <tbody>

  <tr>

   <td width="208"><strong>Objects</strong></td>

   <td width="208"><strong>Properties</strong></td>

   <td width="208"><strong>Verification</strong></td>

  </tr>

  <tr>

   <td width="208"><strong>Client</strong></td>

   <td width="208"></td>

   <td width="208"></td>

  </tr>

  <tr>

   <td width="208"></td>

   <td width="208">Client ID</td>

   <td width="208">&#x2714;</td>

  </tr>

  <tr>

   <td width="208"></td>

   <td width="208">Name</td>

   <td width="208">&#x2714;</td>

  </tr>

  <tr>

   <td width="208"></td>

   <td width="208">Phone number</td>

   <td width="208">&#x2714;</td>

  </tr>

  <tr>

   <td width="208"></td>

   <td width="208">Email</td>

   <td width="208">&#x2714;</td>

  </tr>

  <tr>

   <td width="208"></td>

   <td width="208">DOB</td>

   <td width="208">&#x2714;</td>

  </tr>

  <tr>

   <td width="208"><strong> </strong></td>

   <td width="208">Last Appt.</td>

   <td width="208">&#x2714;</td>

  </tr>

  <tr>

   <td width="208"><strong>Service</strong></td>

   <td width="208"></td>

   <td width="208"></td>

  </tr>

  <tr>

   <td width="208"></td>

   <td width="208">Service ID</td>

   <td width="208">&#x2714;</td>

  </tr>

  <tr>

   <td width="208"></td>

   <td width="208">Serv-name</td>

   <td width="208">&#x2714;</td>

  </tr>

  <tr>

   <td width="208"></td>

   <td width="208">Serv-Desc</td>

   <td width="208">&#x2714;</td>

  </tr>

  <tr>

   <td width="208"></td>

   <td width="208">Serv-Price</td>

   <td width="208">&#x2714;</td>

  </tr>

  <tr>

   <td width="208"><strong>Stylist</strong></td>

   <td width="208"></td>

   <td width="208"></td>

  </tr>

  <tr>

   <td width="208"></td>

   <td width="208">Stylist ID</td>

   <td width="208">&#x2714;</td>

  </tr>

  <tr>

   <td width="208"></td>

   <td width="208">Last name</td>

   <td width="208">&#x2714;</td>

  </tr>

  <tr>

   <td width="208"></td>

   <td width="208">First Name</td>

   <td width="208">&#x2714;</td>

  </tr>

  <tr>

   <td width="208"></td>

   <td width="208">Skills</td>

   <td width="208">&#x2714;</td>

  </tr>

  <tr>

   <td width="208"><strong>Product</strong></td>

   <td width="208"></td>

   <td width="208"></td>

  </tr>

  <tr>

   <td width="208"></td>

   <td width="208">Product ID</td>

   <td width="208">&#x2714;</td>

  </tr>

  <tr>

   <td width="208"></td>

   <td width="208">Prod-Name</td>

   <td width="208">&#x2714;</td>

  </tr>

  <tr>

   <td width="208"></td>

   <td width="208">Prod-Desc</td>

   <td width="208">&#x2714;</td>

  </tr>

  <tr>

   <td width="208"></td>

   <td width="208">Prod-Price</td>

   <td width="208">&#x2714;</td>

  </tr>

  <tr>

   <td width="208"><strong>Purchases</strong></td>

   <td width="208"></td>

   <td width="208"></td>

  </tr>

  <tr>

   <td width="208"></td>

   <td width="208">Purchase- Date</td>

   <td width="208">&#x2714;</td>

  </tr>

  <tr>

   <td width="208"></td>

   <td width="208">Quality</td>

   <td width="208">&#x2714;</td>

  </tr>

 </tbody>

</table>




<h1>User Requirements Specification</h1>

<h3>Entity Types</h3>

<strong>Client Entity Type</strong>:

<ul>

 <li>Client ID: 5 digit identifier meant to be unique within the salon</li>

 <li>First_Name: First name of the client</li>

 <li>Last_Name: Last name of the client</li>

 <li>Client_Phone: Phone number for the client</li>

 <li>Email: Email address for the client</li>

 <li>DOB: Birthday of the client.</li>

 <li>Last_Appt: Derived Attribute for the date of last appointment.</li>

</ul>




<strong>Stylist Entity Type: </strong>

<ul>

 <li>Stylist ID: 3 digit identifier meant to be unique within the salon</li>

 <li>First_Name: First name of the stylist</li>

 <li>Last_Name: Last name of the stylist</li>

 <li>Skills: Multi-value attribute for the skills of the stylist</li>

</ul>




<strong>Service Entity Type: </strong>

<ul>

 <li>Service ID: 4 digit identifier meant to be unique within the salon</li>

 <li>Serv_Name: Name of the service</li>

 <li>Serv_Desc: Short description of the service</li>

 <li>Service Price: Price of the service</li>

</ul>




<strong>Product Entity Type:</strong>

<ul>

 <li>Product ID: 4 digit identifier meant to be unique within the salon</li>

 <li>Prod_Name: Name of the product</li>

 <li>Prod_Desc: Short description of the product</li>

 <li>Prod_Price: Price of the product</li>

</ul>

<h3>Business Verification Rules</h3>

The business rules in the requirement documents are also checked against the ER model as shown the table below




<table width="624">

 <tbody>

  <tr>

   <td width="208"><strong>Relationship</strong></td>

   <td width="208"><strong>Business Rule</strong></td>

   <td width="208"><strong>ER Model</strong></td>

  </tr>

  <tr>

   <td width="208"><strong>Client – Services</strong></td>

   <td width="208"></td>

   <td width="208"></td>

  </tr>

  <tr>

   <td width="208">Client – schedules</td>

   <td width="208">Rule 1</td>

   <td width="208">(0,M)</td>

  </tr>

  <tr>

   <td width="208">Service – schedules</td>

   <td width="208">Rule 2</td>

   <td width="208">(0,M)</td>

  </tr>

  <tr>

   <td width="208"><strong>Client – Stylist</strong></td>

   <td width="208"></td>

   <td width="208"></td>

  </tr>

  <tr>

   <td width="208">Client – assigned</td>

   <td width="208">Rule 1</td>

   <td width="208">(0,M)</td>

  </tr>

  <tr>

   <td width="208">Stylist – assigned</td>

   <td width="208">Rule 2</td>

   <td width="208">(0,M)</td>

  </tr>

  <tr>

   <td width="208"><strong>Client – Product</strong></td>

   <td width="208"></td>

   <td width="208"></td>

  </tr>

  <tr>

   <td width="208">Client – purchased</td>

   <td width="208">Rule 1</td>

   <td width="208">(0,M)</td>

  </tr>

  <tr>

   <td width="208">Product – purchased</td>

   <td width="208">Rule 2</td>

   <td width="208">(0,M)</td>

  </tr>

 </tbody>

</table>

<h3>Relationships</h3>

<strong>Client and Services:</strong>

A client will be scheduled for the services they ask for.




Rule 1: A client can have any number of services rendered and a service can be rendered to multiple people.

Rule 2: During an appointment a service can only be rendered to the assigned client.

<strong> </strong>

<strong>Client and Stylist: </strong>

A client will be assigned a stylist when scheduled for an appointment either by the user’s choice or by with assignment by matching services provided.




Rule 1: A stylist can have multiple clients or none.

Rule 2: A client is scheduled one stylist.

<strong> </strong>

<strong>Client and Product:</strong>

The salon sells various beauty care products. A client can buy as many products as they desire or none at all.




Rule 1: A client can purchase 0 to many products.

Rule 2: A product can be purchased by 0 to many clients

<strong> </strong>

<strong>Stylist and Services:</strong>

A stylist offers specific services that can be offered to the client.




Rule 1: A stylist can have many services offered.

Rule 2: A service can be offered by multiple stylists.

<h1>Model Discussion</h1>

The model supports these processes and keeps track of the dates and times of all scheduled appointments. It provides entities for all of the necessary objects that need to be recorded and tracked as well as keeping track of relationship attributes as needed for the appointments and purchases. All business rules have been verified and modeled accordingly.

<h3>ERD Model</h3>

<h3>Question solve based on the diagram below and above description.</h3>

<ol>

 <li>Database design and creation – implementation of the ER model into a relational database including the design of table structures, testing data and all SQL statements</li>

 <li>_Database application verification – discussion of how application functions, user views, and business processes are supported by the database.</li>

</ol>