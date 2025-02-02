# Dockerized Nginx Web Server

## Overview

This project sets up a virtualized environment using Docker to run a basic Nginx web server. The server serves a simple HTML page inside a Docker container.

## Prerequisites

Ensure you have the following installed on your system:

- [Docker Desktop](https://www.docker.com/products/docker-desktop) (for Windows/macOS)
- [Git](https://git-scm.com/downloads) (optional for version control)

## Setup Instructions

### 1. Clone the Repository

```sh
git clone https://github.com/yourusername/docker-nginx-server.git
cd docker-nginx-server
```

### 2. Build the Docker Image

```sh
docker build -t my-nginx-server .
```

### 3. Run the Docker Container

```sh
docker run -d -p 8080:80 --name nginx-container my-nginx-server
```

### 4. Access the Web Server

Open your browser and go to:

```
http://localhost:8080
```

You should see the webpage served by Nginx.

### 5. Stop and Remove the Container

To stop the running container:

```sh
docker stop nginx-container
```

To remove the container:

```sh
docker rm nginx-container
```

## Project Structure

```
/ docker-nginx-server
  |-- Dockerfile
  |-- index.html
/ README.md
```

- `Dockerfile`: Defines the Nginx container setup.
- `index.html`: Basic HTML page served by Nginx.
- `README.md`: Documentation for the project.

## Technologies Used

- **Docker**: Containerization
- **Nginx**: Web server
- **HTML**: Basic webpage

## Contributing

If you want to contribute or suggest improvements, feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).