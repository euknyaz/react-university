# React University

React University is a sample project demonstrating how to build applications with React, Node.js, and the Lightning Design System. React University is written using ECMAScript 6 on the client and on the server (leveraging the new ES6 support of Node.js 4).

Check out this video for a quick walkthrough:

[![Video](http://img.youtube.com/vi/32Agr6QWmqU/0.jpg)](http://www.youtube.com/watch?v=32Agr6QWmqU)

The back-end is built with **Node.js** using a **Postgres** database. 

The project is written using ECMAScript 6 including ECMAScript 6 modules.

## Local Installation with Docker

Follow the instructions below if you prefer to install the application on your local machine:

1. Install the latest version of Docker and docker-compose

1. Clone this repository

1. Navigate to the **ru-web** directory and run docker-compose:

    ```
    docker-compose up -d
    ```

1. Internally docker-compose should run command

    ```
    npm run docker-start
    ```

    which should execut the following commands defined in package.json:
    ```
    npm install && 
    npm run webpack && 
    node server.js
    ```

1. Database schema is going to be created automatically from init.sql

1. To access PostgreSQL database use the following command:

    ```
    docker-compose exec ru-postgres psql -U postgres ruweb
    ```
    
1. Open a browser and access [http://localhost:5002](http://localhost:5002)
