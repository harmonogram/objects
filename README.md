# objects
Standard objects for API, View, Controller. API Definition files can be used to create stubs in popular languages, like Java, Scala, and Ruby, with just a few clicks.

## Dev Tools 
+ vodAPI.com - describe environment, definition of environment

      + jakie technologie beda uzyte w projekcie ?
      + jakie metody zarzadzania?
      + opis stanowiska pracy dla kazdego uczestnika projektu, jakie opgrogramowanie i sprzet jest potrzebne
            + gitlab / github / bitbucket ?             
      + jakie metody komunikacji?
      + jakie stanowiska
      + jakie etapy w realizacji zlecenia
      
+ APIcra.com - create scripts to create described environment, DevOpsTool

      + skrypty do uzycia w konsoli
      + install
      + create mysql
      + deploy
      
+ unitAPI.com - describe units in project, architecture of code, modules

      + wytyczne dla tworzenia standardow w aplikacji, dla programistow tworzacych kolejne moduly, np na zamowienie

+ DevOpsTerminal, DevOpsTool

      + uzywa skryptow apicra
      + komunikacja z serwerem i zespolem poprzez chat tekstowy, mozliwosc integracji z systemem zarzadzania repozytorium
      

... more info 
https://blog.devtoolsbox.com/index.php/2018/11/08/nowe-narzedzia-dla-devops-team-apicra-unitapi-vodapi/

## Tools API
Codegen

https://github.com/swagger-api/swagger-codegen-generators



## frameworks PHP
Building API

CakePHP


## NodeJS
API SWAGGER CRUD nodejs mysql

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
