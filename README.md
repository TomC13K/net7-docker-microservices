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

# Ports for our created services
- 5000+ localhost
- 8000+ dockerized versions


# Services
- localhost:9001/                     - **portainer**
- localhost:5050/browser/             - **pgAdmin4**
---
- localhost:8000/swagger/index.html   - **catalog.API**
- localhost:8001/swagger/index.html   - **basket.API**
- localhost:8002/swagger/index.html   - **discount.API**