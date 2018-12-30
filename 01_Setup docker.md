# Setup on the Linux

> Auto setup script

```sh
$ sudo wget -qO- https://get.docker.com/ | sh
```

if you was install get.docker.com, the hello-world image will also be installed.
So, We will remove the hello-world image.

```sh
$ sudo docker rm `sudo docker ps -aq`
$ sudo docker rmi hello-world
```
