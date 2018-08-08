# Charlie's Coffee and Sandwich Shop

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This website provides time estimates of inventory delivery for a small food vendor doing business within the city of Boson's subway system.  The vendor delivers the inventory on the subway so it uses a uses Google's direction API to manage arrival times.  Python, Flask, JavaScript, JSON, Socket.IO, HTML5 and CSS will drive the application.  Sqlite will manage the logins, cart registrations, and inventory tracking.

**Business functional summary description**

**Summary:**
	Charlie has an amazing sandwich shop that serves meals from 5am to 6pm. Charlie must keep his inventory storage and shop rental costs low, so he places vendor carts around the city of Boston’s subway system.  He has a kitchen and warehouse located at Downtown Crossing.  Each cart can hold only 50 sandwiches and 10 lbs. of coffee.  Sales at each location range from 30 to 100 sandwiches a day and 20 lbs. of coffee per day.

**Problem:**
	Charlie must use the subway system to deliver inventory to the vendor carts located around the city.  The vendor must know whether his inventory will arrive on time; otherwise, they have to close down, or be able to manage the customer expectations of when the sandwiches or coffee will arrive.

**Requirements for solution:**
* Create a communication system between the vendor carts and warehouse to monitor inventory.
* It will have a username and login page
* Registration of location for the vendor station
* Python, Flask, JavaScript, JSON, Socket.IO, HTML5 and CSS will drive the application.  Sqlite will manage the logins, cart registrations, and inventory tracking.
* Implementation of Bootstrap 4’s mobile responsiveness allows the vendor carts to use their smart phones to communicate.
* The vendor’s have a simple interface that communicates the total number of meals needed from the warehouse
* When the inventory of coffee or sandwiches falls below a certain level an order is typed into the interface to automatically order inventory from the warehouse.  Both Coffee and Sandwiches are ordered to bring the cart back up to the highest inventory level
* Google's directions API is used to communicate to the vender for time of delivery.  The use of this API is key to the communication system.  A message displays to the vendor cart about arrival time.  A countdown then displays on the vendor’s phone to track arrival time.
* Once the delivery is made, the vendor marks it complete and the shop's inventory is marked as inventory sold.
* The API information is located at https://developers.google.com/maps/documentation/directions/start

## Key Components and Design

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This website consists of several pages: index, layout, login, register, and route. It also has a script.js and style.css in the static folder. It has a Flask framework and an application.py file.  The database name is shop.db and is sqlite.



**Open Website**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;At first sign on to the website a database is created with an inventory and user schema.  On subsequent sign-ins, if the database is present, then it will not re-build.  If there are any previous sales in inventory for any vendor, then the data is fetched.  Next the User is presented with a Login and Registration choice on the index page.

**Index.html**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;If the user is not logged in, then the Login and Register buttons appear on the page.  If Login is clicked then the Login page opens, and if Register is clicked, then the Register page opens.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;If the session type is 'shop', then for each vendor in the database the item and value are displayed for sandwiches sold, coffee sold and current deliveries pending delivery.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;If the session type is 'vendor', the order-div is displayed for the vendor to order sandwiches and coffee.





**Event Two -**

**Event Three -**

## Shop 

- Email - shop@final.com
- Password - shop

## There are 4 Vendors

### Vendor A
- Email - vendor_a@final.com
- Password - vendor_a

### Vendor B
- Email - vendor_b@final.com
- Password - vendor_b

### Vendor C
- Email - vendor_c@final.com
- Password - vendor_c

### Vendor D
- Email - vendor_d@final.com
- Password - vendor_d
