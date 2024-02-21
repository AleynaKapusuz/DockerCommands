# DockerCommands

## Install Container :
```
docker pull <containername>
```

## Building a Container :
```
docker run -d --name <name> -p 8080:80<name>
```

## See Running Containers :
```
docker container ls -a
```

## Deleteing a Container
```
docker rm <name>
```

## Show the Image 
```
docker images
```

## Running a Image
```
docker run <ImageID>
```

# ROS and DOCKER
## Opening a ROS Environment with Docker Example
```
docker run --name noetic-aleyna --network host ros:noetic-ros-base-focal sleep infinity
```
## Docker List Container
```
docker ps
```
## Open Terminal
```
docker exec -it noetic-aleyna bash
```
## Install Code Server
```
- apt-get update
- apt-get install curl -y
- curl -fsSL https://code-server.dev/install.sh | sh
- code-server --bind-addr 0.0.0.0:8000
```
## To Save Container Image
```
docker ps # get container id
docker commit <CONTAINER-ID> <IMAGE-NAME>

```

