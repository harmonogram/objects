# unitAPI
1. Wybor odpowiedniej technologii
      + PHP
            + CakePHP
            
      + NodeJs
      + GrpahQL
      + Typescript
      + Mongo / Mysql
      + 
      
2. Stworzenie malych testowych wersji z wlasnym srodowiskiem
3. Deployment, proby zmiany, wypracowanie dokumentacji do stworzenia nowej lepszej wersji
4. Definicje wykonania kolejnych modulow dla Backend, Frontend, DevOps

# ALL
https://medium.com/the-era-of-apis/20-tutorials-on-how-to-create-your-own-api-sorted-by-programming-language-9ad2fa5fc429

## Python
django rest framework
https://www.django-rest-framework.org/

AZURE
https://docs.microsoft.com/en-us/azure/app-service/app-service-web-tutorial-rest-api

SIMPLY
https://www.codementor.io/sagaragarwal94/building-a-basic-restful-api-in-python-58k02xsiq


django-rest-api
https://github.com/gitgik/django-rest-api


Building beautiful REST APIs using Flask, Swagger UI and Flask-RESTPlus
http://michal.karzynski.pl/blog/2016/06/19/building-beautiful-restful-apis-using-flask-swagger-ui-flask-restplus/

    API input validation
    formatting output (as JSON)
    generating interactive documentation (with Swagger UI)
    turning Python exceptions into machine-readable HTTP responses

Why DRF?

    Authentication – From basic and session-based authentication to token-based and Oauth2 capabilities, DRF is king.
    Serialization – It supports both ORM and Non-ORM data sources and seemlessly integrates with your database.
    Great Documentation – If you get stuck somewhere, you can refer to it's vast online documentation and great community support
    Heroku, Mozilla, Red Hat, and Eventbrite are among the top companies using DRF in their APIs.


## GO

      package main

      import (
          "encoding/json"
          "log"
          "net/http"
          "github.com/gorilla/mux"
      )

      // our main function
      func main() {
          router := mux.NewRouter()
          log.Fatal(http.ListenAndServe(":8000", router))
      }

## frameworks PHP
Building API

CakePHP

laravel
https://www.toptal.com/laravel/restful-laravel-api-tutorial


## NodeJS
API SWAGGER CRUD nodejs mysql

Create a single-page web app with REST API backend
SWAGGERIZE
https://docs.microsoft.com/en-us/windows/uwp/get-started/get-started-tutorial-fullstack-web-app


### Express App
Learn Rest API using Express.js and MySQL DB
- easy, appModel.js
https://www.codementor.io/julieisip/learn-rest-api-using-express-js-and-mysql-db-ldflyx8g2

      var todoList = require('../controllers/todoListController');

      // todoList Routes
      app.route('/tasks')
        .get(todoList.list_all_tasks)
        .post(todoList.create_a_task);

       app.route('/tasks/:taskId')
        .get(todoList.read_a_task)
        .put(todoList.update_a_task)
        .delete(todoList.delete_a_task);
        };

Separated Modules
- Modularisation
https://jinalshahblog.wordpress.com/2016/10/06/rest-api-using-node-js-and-mysql/
https://github.com/jinalshah999/nodejsrestapi
      
      app.use('/', routes);
      app.use('/users', users);
      app.use('/Tasks',Tasks);
      
      
Build a Graphql Api for Node & MYSQL 2019— JWT      
-graphQL
https://medium.com/@brianschardt/best-graphql-node-api-template-for-sql-jwt-2018-5e956b715143
https://github.com/brianschardt/node_graphql_apollo_template

            git clone git@github.com:brianschardt/node_graphql_apollo_template.git
            cd node_graphql_apollo_template
            npm install

            //install global packages to run application
            npm i -g nodemon

![deployment](https://cdn-images-1.medium.com/max/1600/1*TRAT1glkPpDFhv-GHCFBNQ.jpeg)

REST API NODE MONGO
https://medium.com/@brianschardt/build-node-mongo-rest-api-2018-jwt-eff0e4f41007
https://github.com/brianschardt/node_rest_api_mongo


REST API NODE MYSQL
https://medium.com/@brianschardt/best-graphql-node-api-template-for-sql-jwt-2018-5e956b715143
https://github.com/brianschardt/node_rest_api_mysql



Building REST APIs with MySQL and Node.js
- generator
https://expressjs.com/en/starter/generator.html

Example
https://github.com/AvanthikaMeenakshi/APIDemo


Passport.js
https://medium.freecodecamp.org/learn-how-to-handle-authentication-with-node-using-passport-js-4a56ed18e81e
- token

Profiling  
https://nodejs.org/en/docs/guides/simple-profiling/
- crypto, hash, salt




## JSON REquest

    {
        "status": true,  <--- Boolean
        "info": "OK",  <--- String, English LABEL, CONSTANS
        "debug": {[  <--- Debug Data Input, Throw Exceptions, format: [{'process', 'variable', 'message'}]
            ...
        ]}
        "input":  {[  <--- Array Input, Variables
            ...
        ]}
        "output": {[  <--- Array Output, Result
            ...
        ]}
    }
