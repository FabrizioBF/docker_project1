Some steps for installing docker and managing some containers.

1.How to install docker.

sudo apt install docker.io -y

sudo systemctl start docker

sudo systemctl enable docker

docker –version

sudo usermod -aG docker ${USER}

sudo su ${USER}


2.Managing the containers.

docker pull debian:10.0

docker pull debian:11.0

docker images

docker inspect 82bd5ee7b1c5

docker inspect 85c4fd36a543

docker run -i -t -d --name buster debian:10.0

docker run -i -t -d --name bullseye debian:11.0
