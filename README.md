# Chat app
It's the time to take a deep dive into Node.js and Express.js by building a chat application with a sign-in system.
<br>In order to implement the sign-in system safely, we will use authentication, which is the act of verifying the identity of a person or process.

<br>Poilerplate comes from FreeCoeCamp, the Advanced Node and Express section. 
<br>Instructions for the lessons start at https://www.freecodecamp.org/learn/quality-assurance/advanced-node-and-express/


## There includes 3 projects
- Registerd User Login
![image](https://user-images.githubusercontent.com/99662300/172035670-8f7d8a59-0403-4d2b-8e9a-6116497ac229.png)

- Registration of New Users
![image](https://user-images.githubusercontent.com/99662300/172035678-a447c432-3134-4c49-8350-6308e6f20818.png)

- Social Authentication to Chat Room
![image](https://user-images.githubusercontent.com/99662300/172035682-72b504d6-f301-4931-9eda-f111a11f63ce.png)


## Built with
- Node.js
- Express.js
- Pug
- MongoDB
- Socket.io


## User Story
- Create middleware to check if the user is logged in before accessing certain routes, and if not, redirect them to homepage.
- To add functionality to log out button, to signing users out. And We also need to take a look at how we can set up a route to return 404 errors.
- To create a registration form, in the POST route, we should create the user's document in the database if it doesn't exist, and then authenticate them using their new details.
- we'll be setting up an Oauth strategy that allows users to log into the site using a Github account and provide information.
- We'll use the 'passport-github' npm package to create a GithubStrategy which will allow the user to login through GitHub and make their profile details available in a callback function.
- The final step we need to add is some database functionality and use the profile information obtained from GitHub to create a user document and serialize it (store in cookie).
- Now that we have access to User information, we can announce to all clients the users that have entered and left the chat, using their name retrieved from cookie.
- To be able to emit and receive chat messages that all clients can see. We can do this by emitting the message to the server, and letting the server emit it to all clients.


## Stretch Goals
- As a registered user, they can login and logout.
- As a user, they can register then logging in as the new user.
- As a user, they can login using a Github account into the chat room. Send and display massages to all online users.
- As a user, they can be announced by the application who has entered or left the chat.

## Live link: https://authentication-advancednode.godherea.repl.co/
