# Task

Create a docker image based on that previously defined Dockerfile and tag it with “{dockerhub_username}/python-greetings-app:latest”
```shell
docker build -t olgamakaranka/python-greetings-app:latest .
```
* `-t` – _tag_ — name and optionally a tag in the name:tag format

---

Run a container based on previously created image with port mapping on host machine
```shell
docker run -d -p 3000:3000 olgamakaranka/python-greetings-app:latest
```
* `-d` – _detach_ — run container in background and print container ID
* `-p` – _publish_ — publish a container’s port(s) to the host
* `-name` – assign a name to the container

---
