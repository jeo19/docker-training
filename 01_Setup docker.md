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

> Using the latest binary

<pre>- When already installed

&nbsp;$ sudo service docker stop
&nbsp;$ sudo wget https://get.docker.com/builds/Linux/x86_64/docker-latest \
    -O $(type -P docker)
&nbsp;$ sudo service docker start

- If you install to new version
  
&nbsp;$ wget https://get.docker.com/builds/Linux/x86_64/docker-latest
&nbsp;$ chmod +x docker-latest
&nbsp;$ sudo mv docker-latest /usr/local/bin/docker
&nbsp;$ sudo /usr/local/bin/docker -d 
</pre>

# Setup on Windows

> Windows 7 or 10 Home (under)

<pre>
Note: If your system does not meet the requirements to run Docker for Windows, you can install Docker Toolbox, which uses Oracle Virtual Box instead of Hyper-V.
</pre>
