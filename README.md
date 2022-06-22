# Big-Data-Management-and-Analysis-in-Physics-Research

## Docker
### build image from Dockerfile
 docker build -t physics .
### run image
docker run --rm -d -p 9001:8888 -p 4040:4040 -e DOCKER_STACKS_JUPYTER_CMD=nbclassic --user root -e GRANT_SUDO=yes  -v ${PWD}:/home/jovyan/ --name container_physics physics  

docker run --rm -d -p 9001:8888 -p 4040:4040 -e DOCKER_STACKS_JUPYTER_CMD=nbclassic --user root -e GRANT_SUDO=yes  -v %cd%:/home/jovyan/ --name container_physics physics

### localhost
open in broswer
http://localhost:9001/
password is 'Fisica2022'
