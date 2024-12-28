# NestJS Dockerized

This is a very minimal NestJS setup using Docker.

## Prerequisites

- Docker
- Docker Compose

## Getting Started

1. Clone the repository:
    ```sh
    git clone https://github.com/khaledxyz/nest-dockerized.git
    cd nest-dockerized
    ```

2. Create a `.env` file in the root directory and add your environment variables.

3. Build and run the Docker containers:
    ```sh
    docker-compose up --build
    ```

4. The NestJS application will be running on port 5000. You can access it at `http://localhost:5000`.

## Docker Compose Configuration

The `docker-compose.yml` file defines the following service:

- `nestjs`: The NestJS application.

### Ports

- `5000:5000`: Maps port 5000 on the host to port 5000 in the container.

### Volumes

- `.:/usr/src/app`: Mounts the current directory to `/usr/src/app` in the container.

### Commands

- `npm run start:prod`: Runs the NestJS application in production mode.

## License

This project is licensed under the MIT License.
