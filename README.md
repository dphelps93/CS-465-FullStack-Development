# CS-465-FullStack-Development

## Architecture

### Compare and contrast the types of frontend development you used in your full stack project, including Express HTML, JavaScript, and the single-page application (SPA).

In this class we used two different styles of creating a web page. One way consisted of creating a multipage web application and the other was a Single Page Application. A multipage website requests a webpage from the server each time the route is followed, where a single page application loads all data into the browser and the browser does the work from there. This may cause single page applications to load slower depending on the complexity and amount of data used for the site. Other tools used in the stack include express, NodeJS, Angular and MongoDB. NodeJS allows for us to perform web server task using JavaScript. Express allows us to create endpoints and handle request to and from the server. Angular is the Front-End tool. It allows us to create dynamic web applications that we don't get using static HTML.

### Why did the backend use a NoSQL MongoDB database?

We used MongoDB because of how well it pairs with the other tools in our stack. It allows us to take JSON data created from our front-end Angular web page and send it directly to the database. Our site used Mongoose as a "glue" between the front-end data and the database on the server.

## Functionality

### How is JSON different from JavaScript and how does JSON tie together the frontend and backend development pieces?

As stated above JSON ties the two together because it is how our data is stored and sent to the server and back. JSON in a nutshell is a way to format data that makes it easy to understand and read. JavaScript is a web-based scripting language. It uses object-oriented principals and can allow for creation of dynamic web sites, where JSON gives us a formatted data type.

### Provide instances in the full stack process when you refactored code to improve functionality and efficiencies and name the benefits that come from reusable user interface (UI) components.

The best example comes from developing the trip card components in the SPA. We refactored the original trip card layout to be able to fit multiple layout styles for future development. By doing so we essentially create a page layout which is reusable and dynamic whenever data is used. This benefits us because we no longer need to develop each card individually. We also have a universal style that is applied whenever a card is created, or data is loaded.

## Testing

### Methods for request and retrieval necessitate various types of API testing of endpoints, in addition to the difficulties of testing with added layers of security. Explain your understanding of methods, endpoints, and security in a full stack application.

Security of applications are very important. We must be sure to authenticate users and give a user’s the correct roles to manage data within the application. Security for this application used a login method and unless a user was logged in then no trips could be Added, Updated, or Delete trip data. Testing that authorization was given was done using POSTMAN. This application allowed for me to send a POST request with trip data to be added to the server. If I did not have a web token applied, which indicated that I was logged in. If I were logged in, I would get a response of 200 indicating success. If I was not logged in, I would get a 401 error which indicated I was not authorized to post. Adding more layers increases testing because we must be sure to add methods that allow us to find errors in the implementation of our end points.

## Reflection

### How has this course helped you in reaching your professional goals? What skills have you learned, developed, or mastered in this course to help you become a more marketable candidate in your career field?

This course has given me the best explanation on how to connect the front end of an application to the server side back-end. In most other courses applications that were created were all console based and did not go into detail on how these applications would work when connected to a server. It also gave me insight to how to create a full stack web application using both multi paged applications and Single Page Applications and how to secure them.
