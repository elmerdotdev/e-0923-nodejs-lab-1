# E-0923 NodeJS Lab Day 1

Goal: Create a CRUD todo application with login functionality

## Instructions

1. Create the backend server using NodeJS and Express
2. Create the frontend using NextJS
3. Use MVC pattern for your backend. You should have two models, one for `todos` and one for `users`. For the users, create an `admin` user and use a hashed password.
4. Place your CRUD functionality in your controllers. Create your API routes using express.Router()
5. On the NextJS frontend, you should have at least these 5 routes:

   - Home `/` - Just use dummy text with log out button
   - Login `/login` - Login form
   - To Dos `/todos` - List of todos with **View** and **Delete** buttons for each todo
   - View Todo `/view/:id` - Show the current todo
   - Add To Do `/new` - Add todo form
   - Edit To Do `/edit/:id` - Edit todo form

6. A user who is not logged in should be able to view, add, or edit any todo. If they are not logged in, they will be redirected to the `/login` page
7. For the login functionality, your backend must be able to receive and send back cookies. You can just call your cookie as `username`
8. Once you are done, push your changes, create a PR from `dev` to `master` and merge

## Properties

- todo: `{ id, task, completed, user }`
- user: `{ id, username, password }`

## References

- [https://github.com/elmerdotdev/e-0923-nodejs-review-w1-w2]
