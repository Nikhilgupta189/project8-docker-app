# Project 8: Build and Run Docker App Locally

## Objective
Build and run a Docker container locally to practice container deployment.

## Technologies Used
- Docker
- Nginx
- HTML
- Linux

## Implementation
1. Created a simple HTML web application.
2. Created a Dockerfile using the Nginx Alpine image.
3. Built a Docker image named `project8-webapp:v1`.
4. Ran a container named `project8-container`.
5. Mapped local port 8080 to container port 80.
6. Verified container status using `docker ps`.
7. Tested the application using `curl`.

## Commands Used

Build image:

`sudo docker build -t project8-webapp:v1 .`

Run container:

`sudo docker run -d --name project8-container -p 127.0.0.1:8080:80 project8-webapp:v1`

Verify:

`sudo docker ps`

Test:

`curl -I http://127.0.0.1:8080`

## Result
Successfully deployed the application inside a Docker container. The container was running, and the application returned HTTP 200 OK.

## Evidence
See the screenshots directory for the successful Docker execution screenshot.

## Conclusion
Successfully demonstrated Dockerfile creation, image building, container execution, and local application testing.
