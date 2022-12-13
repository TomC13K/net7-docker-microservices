# .NET7 docker microservices



## Docker compose spin up n shut down services

```bash
# start up
docker-compose -f docker-compose.yml -f docker-compose.override.yml up -d

# shut down
docker-compose -f docker-compose.yml -f docker-compose.override.yml down

```


## Docker commands

```bash
# check running containers
docker ps

# stop container
docker stop <id-enough 3-4 first chars>

# check stopped containers
docker ps -a

# remove container
docker rm <id-enough 3-4 first chars>

# check all local docker images
docker images

# remove image
docker rmi <full-id>
```


# Services
- localhost:8000/swagger/index.html   - **catalog.API**
- localhost:8001/swagger/index.html   - **basket.API**