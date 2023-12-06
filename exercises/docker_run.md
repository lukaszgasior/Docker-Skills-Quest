# Docker Run Exercises
## Overview
The "Docker Run" category focuses on the essential `docker run` command, a cornerstone of Docker container management. These exercises aim to enhance your skills in creating and configuring Docker containers. You'll explore various options and parameters of the `docker run` command, gaining hands-on experience in managing containers for different requirements. This category is perfect for both beginners and experienced users to practice and refine their Docker container deployment skills.

Remember, practice is key to mastering Docker!

## Exercises

### 1. Run image called `hello-world`

<details>
<summary>solution</summary>
<pre>
<code>
docker run hello-world
</code>
</pre>
</details>

### 2. Run image called `nginx` in version `1.25.3`

<details>
<summary>solution</summary>
<pre>
<code>
docker run nginx:1.25.3
</code>
</pre>

press CTRL+C to stop container
</details>

### 3. Display a list of containers

<details>
<summary>solution</summary>
<pre>
<code>
docker ps
</code>
</pre>
</details>

### 4. Display a list of all containers (including stopped containers)

<details>
<summary>solution</summary>
<pre>
<code>
docker ps -a
</code>
</pre>
</details>

### 5. Run image called `nginx` in detached mode

<details>
<summary>solution</summary>
<pre>
<code>
docker run -d nginx
</code>
</pre>
</details>

### 6. Stop container created in excersise no 5

<details>
<summary>solution</summary>
<pre>
<code>
docker ps

docker container stop CONTAINER_NAME
</code>
</pre>
</details>


### 7. Run image called `nginx` in detached mode. Container should be automatically deleted once stopped.

<details>
<summary>solution</summary>
<pre>
<code>
docker run -d --rm nginx
</code>
</pre>
</details>

### 8. Run image called `nginx` in detached mode. Limit container memory to 500Mb

<details>
<summary>solution</summary>
<pre>
<code>
docker run -d --memory 500M nginx
</code>
</pre>
</details>

### 9. Run image called `nginx` in detached mode. Limit container soft memory to 256Mb

<details>
<summary>solution</summary>
<pre>
<code>
docker run -d --memory-reservation 256M nginx
</code>
</pre>
</details>