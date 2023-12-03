# Docker:

`docker --version` check if docker is already installed

`docker compose version` check if docker compose is installed

`docker ps` The list all running containers

`docker build -t my-postgres .` Build the custom image

`docker build -t issues-tracker .` Docker build command example

`docker-compose up` Run the container

`docker-compose up -d` Run the container in the background

`docker-compose down` Stop the container service, remove the containers associated with the service

`docker compose down -v` with removing volumes

# Access the container:

`docker exec -it postgres psql -U postgres`

--interactive -i Keep STDIN open even if not attached

--tty -t Allocate a pseudo-TTY

## Other useful flags:

--detach -d Detached mode: run command in the background

--detach-keys Override the key sequence for detaching a container

--env -e API 1.25+ Set environment variables

--env-file API 1.25+ Read in a file of environment variables

# psql

`\du` show roles

`\l` show databases

`\dt` show tables

`\q` quit psql

# Commands

1. `docker build -t issues-tracker .`
2. `docker-compose up`

# Others

Host name should be container_name (e.x. "postgres") to connect a database in the container.

Host name shuld be `host.docker.internal` to connect to Postgres running on the host machine from the container.
