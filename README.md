# Building a NodeJS Web App

## Web Frameworks

- [Express](https://expressjs.com/)
- [Feathers](https://feathersjs.com/)
- [Hapi](https://hapijs.com/)
- [Koa](https://koajs.com/)

## Authentication / Authorization Material

### Overviews
- [here](https://hackernoon.com/your-node-js-authentication-tutorial-is-wrong-f1a3bf831a46) is a good article to read to get a sense of common mistakes made in NodeJS applications with authentication

### Services

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
