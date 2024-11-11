# Microservice with Go

This project is a simple web microservice developed in **Golang**. It serves two main endpoints that respond with basic messages. The project includes a Docker configuration for easy deployment.

## Requirements

- **Golang** (if running locally)
- **Docker** (optional, for containerized execution)

## Project Structure

- `main.go`: Contains the Go application code that defines two endpoints.
- `Dockerfile`: Contains instructions to build a Docker image for the service.

## Endpoints

1. **/hello**: Responds with a greeting that includes the requested URL path.
2. **/WeatherForecast**: Responds with a weather forecast message.

## How to Run the Project

### Running Locally

1. Clone the repository and navigate to the project directory.
2. Run the service with:

    ```bash
    go run main.go
    ```

3. The service will be available at `http://localhost:8081`.

### Running with Docker

1. Build the Docker image:

    ```bash
    docker build -t go-microservice .
    ```

2. Run the Docker container:

    ```bash
    docker run -p 8081:8081 go-microservice
    ```

3. The service will be accessible at `http://localhost:8081`.

## Example Responses

- **GET /hello**: Returns a greeting message that includes the path requested.
- **GET /WeatherForecast**: Returns a message saying, “Today is gonna be a great cloudy day for a go service!”

## Notes

Make sure that port **8081** is available on your machine before starting the service.

---

## DockerHub
https://hub.docker.com/repository/docker/paito16/goservice/general
