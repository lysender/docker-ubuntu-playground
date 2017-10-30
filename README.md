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

### Extra software package

This image contains `supervisor` and some python packages required by `supervisor`. Too lazy to find a better entry script, so for now, we are stuck to:

~~~
CMD ["/usr/bin/supervisord", "-n"]
~~~

### Contributing

Pull requests are welcome!

