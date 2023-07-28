# Link Shortener Application 

This application provides the functionality to convert long URLs into short URLs. Users can sign up, login, convert their URLs and view/update their converted URLs. It also shows the total clicks made on the short URLs. 

We will be using Node.js for backend and MongoDB as our database. You can use any front-end technology you prefer.

## Requirements

- Node.js
- MongoDB
- Front-end technology (React, Vue, Angular, or others)
- Basic understanding of HTML, CSS, and JavaScript

## Steps to Follow

1. **Setup Node.js & MongoDB:**
   - Install Node.js & MongoDB on your machine.
   - Initialize a new Node.js project with `npm init`.
   - Install required packages using npm i.e., express, mongoose, bcrypt, jsonwebtoken, etc.

2. **Backend API Setup:**
   - Setup your express server in your Node.js project.
   - Connect MongoDB using Mongoose.
   - Create Models for User and Url.
   - Create routes for User signup, User login, URL conversion, updating URL, and viewing URL.

3. **User Signup & Login:**
   - Create a POST route '/signup' where users can sign up with their email and password. Hash the password before storing it to the database.
   - Create a POST route '/login' where users can login with their email and password. Compare the hash password with the user's input. If the credentials are valid, generate a JWT token and send it in the response.
   
4. **URL Conversion:**
   - Create a POST route '/shorten' where users can send their long URL in the request. Use any URL shortening algorithm to convert the long URL to a short one. Store the short URL and its corresponding long URL in the database. The short URL should be associated with the user who created it.
   
5. **Update and View URL:**
   - Create a PUT route '/update-url' where users can update their long URL. The corresponding short URL should remain the same.
   - Create a GET route '/user-urls' where users can view their URLs. This should return all the URLs created by the user, along with the total click counts for each short URL.
   
6. **Front-End Setup:**
   - Setup your front-end application using the technology of your choice.
   - Create interfaces for user signup, login, URL conversion, updating URL, and viewing URL.

7. **Connecting Frontend and Backend:**
   - Make sure your frontend and backend can communicate with each other. Use fetch or axios to send HTTP requests from your frontend to your backend.

## Expected Deliverables

1. A link to the Github repo containing the application code.
2. A document outlining any special instructions needed to run the application, such as environment variables or config files.
3. A deployed version of the application (optional, but highly encouraged). You can use Heroku, Netlify, Vercel, or any platform you prefer.

## Hints

- Keep your code clean and well-commented. This will help others (and future you) understand what's going on.
- Use version control (git). Regularly commit and push your code to GitHub.
- Try to break down the problem into smaller tasks. This will make it easier to manage and less overwhelming.

Good luck with your implementation. We look forward to seeing your solution!
