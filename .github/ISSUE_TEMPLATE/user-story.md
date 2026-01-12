As a DevOps Engineer
I need to automate the build, test, and deployment process using a CI/CD pipeline
So that application changes can be delivered faster, reliably, and with minimal manual intervention

Details and Assumptions
The application source code is hosted in a Git-based repository 
The application is containerized using Docker.
Jenkins is used as the CI/CD tool.
Builds are triggered automatically on every code push.
Docker images are stored in a container registry.
The application is deployed to a Linux-based server (or cloud VM).
Basic monitoring and logging are enabled to verify deployment success.

Acceptance Criteria
Given the developer pushes code to the main branch
When the CI/CD pipeline is triggered
Then the application should be built successfully

Given the build is successful
When automated tests are executed
Then all tests should pass without errors

Given the tests have passed
When a Docker image is created
Then the image should be tagged and pushed to the container registry

Given the Docker image is available in the registry
When the deployment stage is executed
Then the latest version of the application should be deployed to the server

Given the deployment is complete
When the application health check is performed
Then the application should be running and accessible
