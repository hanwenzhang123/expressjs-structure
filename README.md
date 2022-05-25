# EexpressJS Structure

# src folder
- houses the source code

## configs
- keeps all the configs needed for the application

#### db.config.js
- if the app connects to a database, the configuration for the database

#### general.config.js
- other configurations like the number of records to show on each page for pagination 

## controllers
- house all the controllers needed for the application
- these controller methods get the request from the routes and convert them to HTTP responses with the use of any middleware as necessary.

## middlewares
- segregate any middleware needed for the application in one place
- can be middleware for authentication, logging, or any other purpose.

## routes
- a single file for each logical set of routes
- there can be routes for one type of resource. 

## models
- data models required for the application
- depend on the datastore used if it is a relational or a non-relational (NoSQL) database.
- will have data models defined as per its requirement.

## services
- include all the business logic
- represent business objects and can run queries on the database
- even general services like a database can be placed here.

## utils
- all the utilities and helpers needed for the application
- a place to put shared logic
- a simple helper to calculate the offset for a paginated SQL query can be put in a helper.util.js file in this folder


# test folder
- has all the testing code in it

## unit
- unit tests

#### helper.util.test.js 
- placed inside the utils folder in the unit folder

## integration
- integration tests.


# others
## .env
- .env file to keep the secrets safe and different per deployment environment


