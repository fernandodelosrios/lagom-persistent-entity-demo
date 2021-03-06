# lagom-persistent-entity-demo

> This is a simple lagom application which is used to create user and fetch the details of existing users.
> Lagom's persistent entity is used to handle data persistence for the microservice.

Steps to follow to run this application:

- Open the terminal.
- Clone the project ```git clone git@github.com:DivyaDua/lagom-persistent-entity-demo.git```.
- ```cd lagom-persistent-entity-demo```.
- Execute ```sbt clean compile```.
- Run the cassandra on your localhost, since embedded cassandra is being disabled here.
- Run the application using ```sbt runAll```.

You can check which services are up by hitting ```http://localhost:8000/services```. There, you can see that along with cassandra and kafka, service named 'user_service' is also running.

You can now hit the service using postman -

- To create a new user, hit the service with a POST call using URL - http://localhost:9000/user/create/:id/:name.
  You can give id and name of your choice.

- To fetch user details, hit the service with a GET call using URL - http://localhost:9000/user/details/:id.
  You can give the id for which you want to retrieve the details.




