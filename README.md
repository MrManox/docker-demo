# Docker Demo

## Installation: 

```shell
git clone https://github.com/MrManox/docker-demo
git submodule init
git submodule update
```

### Docker-Commands:
- show images: ```docker images```
- show containers: ```docker ps -a```
- remove all images and containers: ```docker system prune -a```
- build image from dockerfile: ```docker build -f <name of dockerfile> -t <imagename>:<tagname> <path>```
- create container from image ```docker run [OPTIONS] <image-id>```
  - map ports to host: ``` -p <hostport>:<containerport>```
  - interactive: ```-it```
  - detach from console: ```-d```
  - name container: ```--name <containername>```
- stop container: ```docker stop <container-id>```
- delete container: ```docker rm <container-id>```
- delete image: ```docker rmi <image-id>```
- execute command in container: ```docker exec <container-id> <command>```
  - get shell of container: ```docker exec -it <container-id> sh```
- start docker-compose: ```docker-compose up [OPTIONS]```
  - rebuildbuild images: ```--build```
  - detach from console: ```-d```
- stop docker-compose: ```docker-compose stop```
