# E-0923 NodeJS Lab Day 1

Goal: Create a CRUD todo application with login functionality

## Instructions

1. Create the backend server using NodeJS and Express. Install the required packages:

   - express
   - cors
   - bcrypt
   - cookie-parser

2. Create the frontend using NextJS
3. Use MVC pattern for your backend. You should have two models, one for `todos` and one for `users`. For the users, create an `admin` user and use a hashed password.
4. Place your CRUD functionality in your controllers. Set up your middlewares and  create your API routes using express.Router()
5. On the NextJS frontend, you should have at least these 5 routes:

   - Home `/` - Just use dummy text with log out button
   - Login `/login` - Login form
   - To Dos `/todos` - List of todos with **Edit** and **Delete** buttons for each todo
   - Add To Do `/todos/new` - Add todo form
   - Edit To Do `/todos/edit/:id` - Edit todo form

6. A user who is not logged in should not be able to view, add, or edit any todo. If they are not logged in, they will be redirected to the `/login` page
7. For the login functionality, your backend must be able to receive and send back a `username` cookie
8. Once you are done, push your changes, create a PR from `dev` to `master` and merge

## Model Properties

- todo: `{ id, task, completed, user }`
- user: `{ id, username, password }`

## Resources

- [https://github.com/elmerdotdev/e-0923-nodejs-review-w1-w2]
