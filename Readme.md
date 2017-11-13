docker run centos 
docker ps -a

docker run centos uname -a
docker ps -a
docker restart ID

docker run -it centos bash
docker exec -it ID bash

docker stop ID
docker rm ID

docker images
docker rmi ID

FROM centos
RUN touch /tmp/hello.txt
CMD while [ 1 = 1 ]; do echo "Test" && sleep 3; done

docker build -t my_docker_image .

docker run -d my_docker_image
