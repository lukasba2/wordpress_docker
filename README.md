# WordPress Docker Setup

This repository contains a Dockerfile for setting up a WordPress instance with SSL support using Docker.

## Prerequisites

Before you begin, make sure you have Docker installed on your system. You can download and install Docker from the [official Docker website](https://www.docker.com/get-started).

## Setup Instructions

1. **Clone this repository to your local machine:**

    ```bash
    git clone <repository-url>
    ```

2. **Navigate to the cloned repository:**

    ```
    cd wordpress-docker-setup
    ```

3. **Build the Docker image:**

    ```
    docker build -t wordpress-docker .
    ```

4. **Run the Docker container:**

    ```
    docker run -d -p 80:80 -p 443:443 wordpress-docker
    ```

5. **Open your web browser and go to [https://localhost](https://localhost) to access the WordPress site.**

6. **Follow the WordPress setup wizard to complete the installation.**

## Customization

You can customize the WordPress installation by modifying the Dockerfile and default-ssl.conf files

## Notes

- The SSL certificate used is self-signed and is intended for development or testing purposes only.

