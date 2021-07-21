## Setup

### Setup docker
Docker and docker-compose must be installed to run this. Follow instructions here:
https://docs.docker.com/engine/install/
https://docs.docker.com/compose/install/

On Amazon Linux 2:
```
sudo yum update -y
sudo yum install docker
sudo service docker start
sudo chkconfig docker on
sudo usermod -a -G docker ec2-user

sudo curl -L --fail https://github.com/docker/compose/releases/download/1.29.2/run.sh -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
```

### Install git
https://www.atlassian.com/git/tutorials/install-git

On Amazon Linux 2:
```
sudo yum install git -y
```

### Git Clone
git clone https://github.com/kirillian/kirilliantv-containers.git

### cd into the appropriate directory
`cd kirilliantv-container/minecraft`

### Create the .env config file
Copy the example file:
`cp .env.example .env`

In the newly created `.env` file, you need to update the SEED (or remove the line altogether) and RCON_PASSWORD variables

### Run the server
To run the server, run `docker-compose up -d`

### Stopping the server
`docker-compose stop`

## References
Configuration documentation can be found here:
https://github.com/itzg/docker-minecraft-server/blob/master/README.md
