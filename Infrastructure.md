# Udagram On AWS Using CircleCI

## Infrastructure

This file will describe how continuous integration and
continuous deployment to AWS cloud services are implemented in
the project. The project has the following infrastructure:

- Frontend (AngularJS, S3 Bucket) - Fetches data
- Server (NodeJS, Elastic Beanstalk) - Handles frontend requests and runs queries on the database
- Database (PostgreSQL, RDS) - Stores the data being passed by the server

Using the frontend, the user makes requests to the server.
The server handles the request and runs the respective database
queries expected from a route.

## Authors

- [@Youssef Hany](https://www.github.com/youssef-hany)
