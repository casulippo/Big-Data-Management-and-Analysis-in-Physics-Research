# Big-Data-Management-and-Analysis-in-Physics-Research
Questo progetto è stato fatto per il completamento del corso di Big Data Management and Analysis in Physics Research

## Docker
### Costruisci l'immagine
 docker build -t physics .
### Lancia il container
docker run --rm -d -p 9001:8888 -p 4040:4040 -e DOCKER_STACKS_JUPYTER_CMD=nbclassic --user root -e GRANT_SUDO=yes  -v ${PWD}:/home/jovyan/ --name container_physics physics  

oppure

docker run --rm -d -p 9001:8888 -p 4040:4040 -e DOCKER_STACKS_JUPYTER_CMD=nbclassic --user root -e GRANT_SUDO=yes  -v %cd%:/home/jovyan/ --name container_physics physics

Apri il tuo broswer in questo indirizzo
http://localhost:9001/
password is 'Fisica2022'
