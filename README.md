# About This Project

This project serves as a boilerplate for fullstack react redux and mongoDB express applications, this includes **redux store along with auth,users,and profile reducers and actions**, **Fully **, a reducer for **CRUD actions** which performs requests to [https://jsonplaceholder.typicode.com](https://jsonplaceholder.typicode.com) which will response with an API which the components will store and render.
Feel free to add in features, fix bugs and use it for your projects.
This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).
This is a project that I have invested a lot of time. Learned all the technologies incorporated along with this application along as I build this application. Have been a great learning experience

# How this project works

 ## Front End
  In the Front end I bootstraped the app using ` npx create-react-app ` from there, I created all the layouts, components and validations for the forms.
  Protection on privates routes, using json web token from the backend which expires in 
  I used redux to gain an overview of the application-level states such as Auth, User/s, and Profile/s.
  Using thunk, I've set up a success and failed state where if the fetching of my data from the backend fails the front end will reconstruct accordingly.
 
 ## Back End
  In the Back end I used express as my node backend framework, Routing and server side validation are also in the routes folder and validation folder, respectively.
  Used passport for authentication along with json web token stored in the local storage which is associated with an account to ensure private routing are protected and to also ensure that users are automatically logged out after an hour of gaining a token.
  I used MongoDB Atlas as my cloud database.
  
  Back end has the following routes:
  
  ### PRIVATE API ROUTES:
    POST /api/profiles/:user_id
    POST /api/posts/
    POST /api/posts/comment/:post_id
    POST /api/posts/like/:post_id
    POST /api/posts/unlike/:post_id
    DELETE /api/posts/:post_id
    DELETE /api/profiles/:user_id
    DELETE /api/posts/comment/:post_id/:comment_id
  ### PUBLIC API ROUTES:
    POST /api/users/register
    POST /api/users/login
    GET /api/posts/:post_id
    GET /api/posts/all
    GET /api/profiles/all
    GET /api/profiles/:user_id
    GET /api/profiles/:handle
    GET /api/users/current
    

## How to use this project
In your Terminal,
  1. ` npm client-install ` to install all the dependencies on the frontend, and configurations for this boilerplate.
  2. ` npm install ` to install all the dependencies on the backend, and configurations for this boilerplate.
  3. ` npm start ` to start your backend application which will run your localhost in the port 5000 /[http://localhost:3000](http://localhost:3000).
  3. ` npm client ` to start your frontend application which will run your localhost in the port 3000 /[http://localhost:3000](http://localhost:3000).
  4. Perform actions and add in your customizations to the app.

## Available Scripts

In the project directory, you can run:

### `npm client-install` and `npm install`

  To install both of the dependencies in the front end and backend, once done move the next step

### `npm client`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `npm start`

Runs the server in the development mode.<br />
Open [http://localhost:5000](http://localhost:5000) to view it in the browser.


### `npm test`

Launches the test runner in the interactive watch mode.<br />

### `npm run build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!


