Reference minecraft docker server documentation here:

https://github.com/itzg/docker-minecraft-server

### Setup docker
Docker and docker-compose must be installed to run this. Follow instructions here:
https://docs.docker.com/engine/install/
https://docs.docker.com/compose/install/

### Git Clone
git clone https://github.com/kirillian/kirilliantv-containers.git

### cd into the appropriate directory
`cd kirilliantv-container/minecraft`

### Create the .env config file
Copy the example file:
`cp .env.example .env`

Configuration documentation can be found here:
https://github.com/itzg/docker-minecraft-server/blob/master/README.md

### Run the server
To run the server, run `docker-compose up -d`

### Stopping the server
`docker-compose stop`
