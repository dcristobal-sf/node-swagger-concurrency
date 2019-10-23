# node-swagger-concurrency
Heroku Example for WEB_CONCURRENCY with Node and Swagger. This example demonstrates how to apply Concurrency to [Node.js](https://nodejs.org) server applications created with Swagger as part of [Heroku](https://www.heroku.com/platform) Twelve-Factor App methodology.

## Overview
This server was generated by the [swagger-codegen](https://github.com/swagger-api/swagger-codegen) project.  By using the [OpenAPI-Spec](https://github.com/OAI/OpenAPI-Specification) from a remote server, you can easily generate a server stub.  This is an example of building a node.js server.

This example uses the [expressjs](http://expressjs.com/) framework.  To see how to make this your own, look here:

[README](https://github.com/swagger-api/swagger-codegen/blob/master/README.md)

### Running the server
To build & run the server as default 1 process, run:

```
npm start
```

To build & run the server with 4 concurrent processes, rin:

```
WEB_CONCURRENCY=4 npm start
```

The build process fetches all required dependencies to run this server. This is needed for deployment to Heroku platform, for Node buildpack to assemble this app.

To run the server, run:

```
WEB_CONCURRENCY=4 node index.js
```

To view the Swagger UI interface API docs:

```
open http://localhost:8080/docs
```

This project leverages the mega-awesome [swagger-tools](https://github.com/apigee-127/swagger-tools) middleware which does most all the work.
