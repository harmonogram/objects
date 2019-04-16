# objects
Standard objects for API, View, Controller. API Definition files can be used to create stubs in popular languages, like Java, Scala, and Ruby, with just a few clicks.


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
