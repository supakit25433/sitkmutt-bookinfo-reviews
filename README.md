# Reviews service

running on port 8082

## What change in Dockerfile

change gradle version to 7.2.0-jdk11 and websphere-liberty version to 21.0.0.9-kernel-java8-ibmjava

## How to run with Docker

```bash
# Build Docker Image for reviews service
docker build -t reviews .

# Run reviews service on port 8082
docker run -d --name reviews -p 8082:9080 reviews
```

* Test with path `/reviews/1` and `/health`

## How to run with Docker Compose

```bash
# use for build and run in first use
docker-compose up

# use for rebuild docker image and run
docker-compose up --build
```