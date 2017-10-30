# docker-ubuntu-playground
Ubuntu (16.04) Xenial Base Image for testing software packages in Ubuntu

## Usage

### Creating and running container

~~~
sudo docker run --name ubuntu-playground -d lysender/ubuntu-playground
~~~

### Testing inside the container

~~~
sudo docker exec -it ubuntu-playground bash
# Do whatever you want
# Looking for the right package name?
apt-cache search awscli
# Not sure about the config path?
ls /etc/nginx/*
~~~

