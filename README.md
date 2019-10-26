# FullstackMonorepo

Application based on the Kelvin Mai course [Ideas App](https://www.youtube.com/watch?v=NF9Xn4g5MJY&list=PLBeQxJQNprbiJm55q7nTAfhMmzIC8MWxc)

This project was generated using [Nx](https://nx.dev).

## Stack

- Database - PostgreSQL
- REST API - NestJS
- GraphQL API - NestJS
- Rest Frontend - Angular with NGRX

## Running applications

> Running postgres via docker

```
docker run -d -ePOSTGRES_USER=postgres -ePOSTGRES_PASSWORD=postgres -ePOSTGRES_DB=test -p5432:5432 --name postgres  postgres:10.4-alpine
```

> Creating a database 

```
docker exec -it postgres bash
bash-4.4# su - postgres
323fdaadc000:~$ psql 
psql (10.4)
Type "help" for help.

postgres=# CREATE DATABASE fullstack;
CREATE DATABASE
postgres=# ^D
323fdaadc000:~$ ^D
bash-4.4# ^D
```

> Setting the environment variables

```
export API_DB_USERNAME=postgres
export API_DB_PASSWORD=postgres
export API_DB_NAME=fullstack
export SECRET=SuperComplexStringSequenceNeededHere
```



Run `ng serve` to start client server. 
Run `ng serve api` to start api server. 

Run `npm start` to start both servers. 

## Swagger

http://localhost:3333/swagger/


## GraphQL playground

http://localhost:3333/graphql/

## Running unit tests

Run `ng test` to execute the unit tests via [Jest](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Cypress](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
