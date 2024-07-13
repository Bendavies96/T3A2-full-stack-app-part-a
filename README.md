# T3A2-full-stack-app-part-a

R1 Description of your website, including:

- Purpose

  Willem

- Functionality / features

  - Generator link to event (dynamically)
    "https://an-app-name.com.au/events/id="eventid"
  - Email users welcome and reset password
  -

- Target audience

  Jimmy

- Tech stack
  We have opted for a full stack MERN web application including:

Front end:
ReactJS
Javascript
HTML5
CSS3

Database:
MongoDB
Mongoose

Back end:
Node.js
ExpressJS

Package Management:
npm

Testing:
Insomnia
Jest
Github Actions
React Testing Library

Diagrams and Design:
draw.io

Project Management:
Trello

DevOps:
Visual Studio Code
Git
GitHub

Hosting:
Netlify - front end hosting
Server - either AWS or Render

Email Service:
Google Console

---

R2 Dataflow Diagrams BEN

User Creation Sqenence Diagram

1. The Client Enters there Username, email, password, country (for language selection), This is then posted to the server.
2. The Server then receives the HTTP request, checks that all the required information is in the JSON body and formatted correctly.
3. The database now receives the users data from the Server.
4. The Server recieves a response from the database including the user ID, Email and Username. This is now used to create a JWT Token for the user.
5. The JWT token is now passed to the user.
6. The Server Now Runs a function to create a welcome email for the user. It requires the Oauth details from the enviroment variables The Username and Email of the user.
7. Google Console recieves a request to send an email. Google validates the Oauth keys and returns an error or successful response.
8. The User can now view this in there Email Client.

User Resets Password

1. The Client Enters there email address, then posts this to the Server.
2. The Server Verifies the JSON data is correctly formatted and complete.
3. The database checks if the users email exists and creates a single use access token for the user with 20 minute timestamp.
4. The Link to reset the users password is created with a single use access token.
5. The email is created including the HTML Template, link to reset password.
6. A request to google is sent with the Oauth keys, google response with a sucess or failure.
7. User can now access the Link to reset there password from there Email Client of choice.

---

R3 Application Architecture Diagram BEN

---

R4 User Stories Everyone

---

R5 Wireframes for multiple standard screen sizes, created using industry standard software Willem

---

R6 Screenshots of your Trello board throughout the duration of the project
