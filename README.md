# PWN-DOCKER

building
```
sudo docker build -t my_docker_image .

sudo docker images
sudo docker rmi <IMAGE_ID>
sudo docker run -d -p 7182:7182 --name my_docker_container my_docker_image

sudo docker ps (-a)
sudo docker exec -it my_docker_container /bin/bash
sudo docker exec -u root -it my_docker_container /bin/bash
```
