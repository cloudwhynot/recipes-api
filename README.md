# recipes-api

### Description
RESTful API with Express. Authentication provided by Passport.js using JSON Web Tokens.

### Installation
To install all dependencies, run the following command in your terminal:
```shell
npm install
```

### Environment Variables
Also you will need to add the `JWT_SECRET='your_secret_token'` environment variable to your `.env` file.
To create one you can run the following command in your terminal:
```shell
node -e "const jwt = require('jsonwebtoken'); const crypto = require('crypto'); const token = jwt.sign({ data: crypto.randomBytes(23).toString('hex') }, 'your_secret_key'); console.log(token);"
```

### Usage
To start the application, run:
```shell
npm start
```
