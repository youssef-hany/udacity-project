## Pipeline Process

The pipeline is implemented through CircleCI by providing:

- config.yml - Contains all the instructions of the process on the pipeline.
- Environment Variables are set in CircleCI to ensure they are kept safe.

This pipeline automates the integration and the deployment keeping the project linked with github.
So that anytime there is a new commit to the master branch the pipeline is automatically triggered to run installations, build and deploy frontend and backend through CircleCI to their AWS respective services
