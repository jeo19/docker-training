# Lifecycle of the docker

> create container

<pre>
- docker run [Image name or ID]
</pre>

> Stop the container

<pre>
- docker stop [Image name or ID]
</pre>

> Start container

<pre>
- docker start [Image name or ID]
</pre>

> Restart container

<pre>
- docker restart [Image name or ID]
</pre>

> Remove container

<pre>
- docker rm [Image name or ID]
</pre>

> Connect the running container

<pre>
- docker attach [Image name or ID]
</pre>

# Command to output related information.

> Shows a list of running containers (The docker ps -a command shows a list of running and stop containers)

<pre>
- docker ps
</pre>

> Shows a all info of specific container to including ip

<pre>
- docker inspect
</pre>

> Output a log of container

<pre>
- docker logs
</pre>

> Output the events of container

<pre>
- docker events
</pre>

> Shows the info of connected port

<pre>
- docker port
</pre>

> Shows the running process of container

<pre>
- docker top
</pre>

> Shows the changed file on container filesystem.

<pre>
- docker diff
</pre>
