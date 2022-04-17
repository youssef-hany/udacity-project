# Udagram On AWS Using CircleCI

This file will describe how continuous integration and
continuous deployment to AWS cloud services are implemented in
the project. The project has the following infrastructure:

- Frontend (AngularJS, S3 Bucket)
- Server (NodeJS, Elastic Beanstalk)
- Database (PostgreSQL, RDS)

Using the frontend, the user makes requests to the server.
The server handles the request and runs respective the database
queries expected from a route.

## Final Look

The Application is hosted [Here](http://udacityyoussefhany.s3-website-us-east-1.amazonaws.com/)
using AWS S3 bucket static web hosting.

## Frontend

The application uses the following technologies:

- AngularJS - Frontend User Interface.
- S3 bucket - AWS cloud service to host files.

## Backend

The server uses the following technologies:

- Express - Server to manage incoming requests.
- Sequelize - Manages all database interactions.
- AWS Elastic Beanstalk - Hosts the server and runs it in a node environment. [AWS API](http://youssefhanyapi-env.eba-txjztr4p.us-east-1.elasticbeanstalk.com)

## Database

The Database uses the following technologies:

- PostgreSQL.
- AWS RDS Service. - [Database Host](database-2.cxbch9hrjslr.us-east-1.rds.amazonaws.com)

## Pipeline Process

The pipeline is implemented through CircleCI by providing:

- config.yml - Contains all the instructions of the process on the pipeline.
- Environment Variables are set in CircleCI to ensure they are kept safe.
  This pipeline automates the integration and the deployment keeping the project linked with github.
  So that anytime there is a new commit the pipeline is automatically triggered.

## Authors

- [@Youssef Hany](https://www.github.com/youssef-hany)
