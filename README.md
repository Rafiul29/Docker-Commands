
## Docker version
This command is used to get the currently installed version docker
```sh
docker -v 
docker --version
```
## Docker pull
This command is used to pull images fro the docker repository(hub.docker.com)
```sh
docker pull <image name>
docker pull ubuntu
```
## Docker run
This is used to create a container from image
Note: -it (interactive terminal)  -d ( detash)
```sh
docker run -it -d <image name>
docker run -it -d ubuntu
```
## Docker Running container 
```sh
docker ps
```
##  Docker Running and exited container
```sh
docker container ps -a
```
## Docker access the running contaienr 
```sh
docker exec -it <contaier id> bash
```
## Docker stops a running container
```sh
docker stop <container id>
```
## Docker Kill
```sh
docker kill <container id>
```
## Docker commit 
```sh
docker commit <container id> <username/imagename>
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
## Docker Remove container
Delete a stopped container 
```sh
docker container rm <contianer id>
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



