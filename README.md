## Docker version
This command is used to get the currently installed version docker
```sh
docker -v 
docker --version
docker version
```
## Docker info
Display system-wide information
```sh
docker info
```
## Docker pull
This command is used to pull images fro the docker repository(hub.docker.com)
```sh
docker pull <image name>
docker pull ubuntu
```
## Docker run
This is used to create a container from image
Note: -it (interactive terminal)  -d ( detach)
```sh
docker run -it -d <image name>
docker run -it -d ubuntu
```
## Docker container list
```sh
docker container ls
```
## Docker running container 
```sh
docker ps
```
##  Docker running and exited container
```sh
docker container ps -a
```
## Docker access the running container
```sh
docker exec -it <contaier id> bash
```
## Docker start container
```sh
docker contaienr start <container id>
```
## Docker stops a running container
```sh
docker stop <container id>
```
## Docker login
This command is used to login to the docker hub repository
```sh
docker login
```
## Docker Push
Push image to the docker hub repository
```sh
docker push <usernane/image name>
```
## Docker image
The locally stord docker image
```sh
docker image ls
```
## Docker remove container
Delete a stopped container 
```sh
docker container rm <contianer id>
```
## Docker remove multiple container
Delete a stopped container 
```sh
docker container rm <contianer id>  <contianer id> 
```
## Docker remove all container 
Stop the container before attempting removal or force remove
```sh
1. docker container ls -aq
2.docker container rm $(docker container ls -aq)
```
## Docker rmi (removes image by their ID)
delete an image from local storage
```sh
docker rmi <image-id>
```
## Docker Bulid
build an image from a specific docker file
```sh 
docker bulid <path to docker file>
```
## Docker contianer inspect
Docker inspect provides detailed information on constructs controlled by Docker.
```sh
docker container inspect <container id>
```
## Docker port mapping
```sh
docker container run -d -p 3600:80 --name test1 nginx
docker contaienr run -it -d -p 7000:80 --name test2 nginx
```
## Docker rename container 
```sh
docker container rename <container id> <new name>
```
# Docker restart container
```sh
docker container restart <container id>
```
## Docker exec container

```sh
docker container exec  -it <container id> /bin/bash
```
# Docker container kill,attach,wait,pause,unpause,prun,port
## Docker container Kill
```sh
docker container  kill <container id>
```
## Docker container attach
```sh
docker container attach <container id> 
```
## Docker container wait
```sh
dokcer container wait <container id>
```
## Docker container pasuse
```sh
docker container pause <container id>
```
## Docker container unpasuse
```sh
docker container unpause <container id>
```
## Docker container prune
Deleted Containers:
```sh
docker container prune <container id> -f
```
## Docker container Port
```sh
docker container port <container name>
```
# Docker Export/Import Container
## Docker Export
same output two command ,show watch file command (ls -sh)
```sh
docker container export <container id>  >ubuntu_tree.tar
docker container export <container id> -o ubuntu_tree1.tar
```
## Docker Import
```sh
docker image import ubuntu_tree.tar ubuntu1
docker container run -it ubuntu1 /bin/bash
```
## Docker commit 
```sh
docker commit <container id> <username/imagename>
```

