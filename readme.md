# Simple to-do list application

- This is suppose to be just a simple to-do list application.
- The application currently consists only on the backend.
- The app was made for the purpose of practicing some Javacript. I do not recommend using this app in your daily life.
- Maybe in the future, a client side of the app can be developed. 
- Feel free to propose a frontend application that can be useful for this application.

## BACKEND
- Javascript/Nodejs
- Express

### JSON file

- In this application , all the data is stored in JSON files
- The tasks are located in the ``` tasks.json``` file
- The users are located in the ``` users.json``` file
- The file will be created automatically when you start the server.
- Do not delete all the content present in ``` tasks.json```. In order to this API to work this file must have at least an empty array.

### Structure of JSON files

- tasks.json
```
[
  {
  "user":"j4gyxbws",
  "id":"goqfc5ld",
  "description":"Go to college",
  "due":"Saturday",
  "status":"In progress"
  },
  
  {
  "user":"j4gyxbws",
  "id":"jnyub90p",
  "description":"Do math exercises",
  "due":"Tuesday",
  "status":"In progress"
  },

  {
  "user":"4l3jjz9s",
  "id":"i2yse9l3",
  "description":"Programming",
  "due":"Monday",
  "status":"In progress"
  },

```
- users.json
```
  [
    {
    "id":"4l3jjz9s",
    "name":"John",
    "email":"John@gmail.com",
    "password":"123456"
    },
    {
    "id":"j4gyxbws",
    "name":"Sarah",
    "email":"sarah@gmail.com",
    "password":"123456"
    }
  ]
```

### API

The API is structered in certain folders.

- Controllers  - Implementation of endpoins

- HandleJSON -  Handles the data in the JSON files

- Middleware - Contains the middlewares

- Routes - Declaration of endpoints

### Authentication
- The authentication is based on JSON Web Tokens. So everytime you register a user or login, a token will be generated. This token will allow you to get informations about the own currently user and add tasks and manipulate them through requests.

### Scripts

```
npm i - Install the dependencies
```

```
npm start - Run the local server
```

### Observations
 - The user is only allowed to get , create , update and delete a task if authenticated.

 ## What's missing and next steps
 - The frontend part