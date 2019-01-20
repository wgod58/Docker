# Docker?
**Build docker images with ./Dockerfile**
* docker build .

**Strat new container with image**
* docker run -t -i -p 8080:8080 caterpillar/java-tutorial bash
* docker run -it (imageName) bash

**Exec exist container**
* docker exec -it <mycontainer> bash
  
**Copy file to container**
* docker cp foo.txt mycontainer:/foo.txt
* docker cp mycontainer:/foo.txt foo.txtgi

**Commit & push to Docker hub**
* docker commit -m="mytomcay" -a="zed pai" 2c9f59b7fbb8  wgod58/mytomcat
* docker push wgod58/mytomcat

**show container**
* docker ps    //running
* docker ps -a //all container

**list all images**
* docker images //show images



## Containers
* Lifecycle
  * [docker create]() creates a container but does not start it.
  * [docker rename]() allows the container to be renamed.
  * [docker run]() creates and starts a container in one operation.
  * [docker rm]() deletes a container.
  * [docker update]() updates a container's resource limits.
* Starting and Stopping
  * [docker start]() starts a container so it is running.
  * [docker stop]() stops a running container.
  * [docker restart]() stops and starts a container.
  * [docker pause]() pauses a running container, "freezing" it in place.
  * [docker unpause]() will unpause a running container.
  * [docker wait]() blocks until running container stops.
  * [docker kill]() sends a SIGKILL to a running container.
  * [docker attach]() will connect to a running container.
* Info
  * [docker ps]() shows running containers.
  * [docker logs]() gets logs from container. (You can use a custom log driver, but logs is only available for json-file and journald in 1.10).
  * [docker inspect]() looks at all the info on a container (including IP address).
  * [docker events]() gets events from container.
  * [docker port]() shows public facing port of container.
  * [docker top]() shows running processes in container.
  * [docker stats]() shows containers' resource usage statistics.
  * [docker diff]() shows changed files in the container's FS.

## Images
* Lifecycle
  * [docker images]() shows all images.
  * [docker import]() creates an image from a tarball.
  * [docker build]() creates image from Dockerfile.
  * [docker commit]() creates image from a container, pausing it temporarily if it is running.
  * [docker rmi]() removes an image.
  * [docker load]() loads an image from a tar archive as STDIN, including images and tags (as of 0.7).
  * [docker save]() saves an image to a tar archive stream to STDOUT with all parent layers, tags & versions (as of 0.7).

* Info
  * [docker history]() shows history of image.
  * [docker tag]() tags an image to a name (local or registry)

#### reference
  * [官方文件 方便查詢使用的參數](https://docs.docker.com/engine/reference/commandline/docker/)
  * [Docker File 撰寫](https://philipzheng.gitbooks.io/docker_practice/content/dockerfile/instructions.html)
  * [docker-cheat-sheet](https://github.com/wsargent/docker-cheat-sheet)