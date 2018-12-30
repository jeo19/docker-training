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

> Ubuntu

```sh
$ sudo apt-get update
$ sudo apt-get install docker.io
$ sudo ln -sf /usr/bin/docker.io /usr/local/bin/docker
```

> RedHat Enterprise Linux, CentOS

<pre>- CentOS 6
$ sudo yum install http://dl.fedoraproject.org/pub/epel/6/x86_64/epel-release-6-8.noarch.rpm
$ sudo yum install docker-io
</pre>
<pre>- CentOS 7
&nbsp;$ sudo yum install docker
</pre>
<pre>- Run the docker service
&nbsp;$ sudo service docker start
- Run when booting the OS
&nbsp;$ sudo chkconfig docker on
</pre>
