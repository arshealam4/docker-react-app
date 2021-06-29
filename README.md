# Docker React App
This is simple react app to use for docker and docker compose. We have created for development and production environment.

## Requirements

To run this app docker angine and docker compsoe  should be installed.

### Start
- git clone https://github.com/arshealam4/docker-react-app.git
- cd docker-react-app
- Follow the below instruction for docker

### Start Docker Dev
- docker build build -t hello-word-dev .
- docker run -it -p 3000:3000 hello-word-dev
- open it on browser: localhost:3000

### Start Docker Prod
- docker build -f Dockerfile.prod -t hello-world:prod .
- docker run -it -p 3005:3000 hello-word-prod
- open it on browser: localhost:3005

### Start Docker Compose Dev
- docker-compose up -d --build

### Start Docker Compose Prod
- docker-compose -f docker-compose.prod.yaml up -d --build

### Start/Stop/Other

- docker build
- docker run
- docker start
- docker stop
- docker rm id
- docker logs <cointainerId>
- docker exec -it <cointainerId> sh
- delete all container => docker container rm -f $(docker container ls -a -q)
- delete all images => docker images rm -f $(docker images ls -a -q)
- docker-compose build
- docker-compose down
- docker-compose up
- docker-compose stop
- docker-compose start
