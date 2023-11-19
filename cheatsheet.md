# Docker:

`docker --version` check if docker is already installed

`docker compose version` check if docker compose is installed

`docker ps` The list all running containers

`docker build -t my-postgres .` Build the custom image

`docker-compose up` Run the container

`docker-compose up -d` Run the container in the background

`docker-compose down` Stop the container service, remove the containers and volumes associated with the service

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
