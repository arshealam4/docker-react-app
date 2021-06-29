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
- docker build build -t hello-word-prod .
- docker run -it -p 3005:3000 hello-word-prod
- open it on browser: localhost:3005

### start Docker Compose Dev
- docker-compose up -d --build

### start Docker Compose Prod
- docker build -f Dockerfile.prod -t hello-world:prod .

### start/stop

- docker start
- docker stop
- docker rm id
- docker-compose down
- docker-compose up
- docker-compose stop
- docker-compose start
