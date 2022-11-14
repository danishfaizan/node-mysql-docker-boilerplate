# node-mysql-docker-boilerplate

A boilerplate project for setting up MySql, Node.JS and Docker in the dev environment.

## Prerequisites

- Docker

## How to run

```
docker-compose up
```

Call this endpoint to see if it works

```
localhost:3000/users
```

## Alternative ways to run

You can also run the app without docker, just update the `.env` file wtih the correct IP, port and credentials of a mysql server.

```
npm run dev-local
```

You can start a mysql server in docker if needed with

```
docker run -p 3306:3306 --name test-mysql -e MYSQL_ROOT_PASSWORD=root -e  MYSQL_DATABASE=test -d mysql --default-authentication-plugin=mysql_native_password
```

This allows you to avoid using docker-compose.
