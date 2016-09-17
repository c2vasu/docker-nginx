# Docker Compose using Nginx
Sample Docker with Nginx as proxy for static files

### Building images
```
$ cd docker-nginx
$ docker-compose build
```
### Fire up containers
```
$ docker-compose up
```
### Scaling containers
Open new terminal and run the below command.
```
$ docker-compose scale <SERVICE>=4
$ docker-compose scale app=4
```
### Healing
Means re-running containers that have stopped
```
$ docker-compose up --no-recreate
```
### Status of containers
```
$ docker-compose ps
```
### To pull latest version of containers & re-create
```
$ docker-compose pull
$ docker-compose up -d
```
### Logs of the containers
```
$ docker-compose logs
```
### In case you want to run app as stand alone
```
$ cd /app
$ docker build -t app .
$ docker run -p 9000:80 app
```
### Docker-Compose cheat sheet
```
build    Build or rebuild services
help     Get help on a command
kill     Kill containers
logs     View output from containers
port     Print the public port for a port binding
ps       List containers
pull     Pulls service images
rm       Remove stopped containers
run      Run a one-off command
scale    Set number of containers for a service
start    Start services
stop     Stop services
restart  Restart services
up       Create and start containers
```
