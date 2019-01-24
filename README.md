# Building a NodeJS Web App

This document is meant to give a guided tour into building a proper NodeJS Web Application. When building a web application, many things need to be considered:

## Web Frameworks

First, you need to decide on a Web Framework to build on top of (unless you are one of those who wants to build something from scratch, in which case, you should start with the node documentation on the [HTTP](https://nodejs.org/api/http.html) module).

- [Express](https://expressjs.com/)
- [Feathers](https://feathersjs.com/)
- [Hapi](https://hapijs.com/)
- [Koa](https://koajs.com/)

## Authentication / Authorization Material

Authentication is very important to get right and many NodeJS tutorials have misleading or poor practices on how to do this properly. Depending on whether you are building your own solution or you just want to use something that has already been built, there is material below to guide you through the process.

### Overviews
- [Here](https://hackernoon.com/your-node-js-authentication-tutorial-is-wrong-f1a3bf831a46) is a good article to read to get a sense of common mistakes made in NodeJS applications with authentication

### Services

If you are looking for a pre-built solution, here are some places to start:

- [Firebase](https://firebase.google.com/) handles most of authentication for you, including storing passwords, 2-factor authentication, and password reset requests.
- [Auth0](https://auth0.com/) is "Authentication-as-a-service" and includes libraries and tutorials in most languages (including Node)

### Middleware

- [Passport JS](http://www.passportjs.org/) is the most popular library for handling user authentication. It is extensible and has strategies for Facebook, Google, and Twitter logins (and much more...). Passport does not handle all of authentication for you; you still need to handle things such as password hashing / storage, password reset requests, authorization, 2-factor authentication, and rate limiting.
- [Oauth2orize](https://github.com/jaredhanson/oauth2orize) is an alternative to PassportJS that is designed specifically for OAuth workflows

### Password Hashing / Encryption

- [Bcrypt](https://www.npmjs.com/package/bcrypt) is a good node js library for hashing password safely
- [Aargon2](https://www.npmjs.com/package/argon2) is another good node js library for hashing passwords

### JSON Web Tokens (JWT)

- Look [here](https://jwt.io/) for a description of what they are
- Look [here](https://medium.com/@siddharthac6/json-web-token-jwt-the-right-way-of-implementing-with-node-js-65b8915d550e) for a good article on implementing JSON web tokens in NodeJS
- Look [here](https://news.ycombinator.com/item?id=13866883) for criticism on using JWT
