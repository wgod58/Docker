# Docker?

```
	docker build .
	docker cp foo.txt mycontainer:/foo.txt
	docker cp mycontainer:/foo.txt foo.txt
	docker run -t -i -p 8080:8080 caterpillar/java-tutorial bash
	docker run -it (imageName) bash
	docker exec -it <mycontainer> bash
	docker cp foo.txt mycontainer:/foo.txt
	docker cp mycontainer:/foo.txt foo.txt
	docker commit -m="mytomcay" -a="zed pai" 2c9f59b7fbb8  wgod58/mytomcat
	docker push wgod58/mytomcat
  
```

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
  * https://docs.docker.com/engine/reference/commandline/docker/
  * https://github.com/wsargent/docker-cheat-sheet

一个在线编辑markdown文档的编辑器

向Mac下优秀的markdown编辑器mou致敬
````
   for coloring



## MaHua有哪些功能？

* 方便的`导入导出`功能
    *  直接把一个markdown的文本文件拖放到当前这个页面就可以了
    *  导出为一个html格式的文件，样式一点也不会丢失
* 编辑和预览`同步滚动`，所见即所得（右上角设置）
* `VIM快捷键`支持，方便vim党们快速的操作 （右上角设置）
* 强大的`自定义CSS`功能，方便定制自己的展示
* 有数量也有质量的`主题`,编辑器和预览区域
* 完美兼容`Github`的markdown语法
* 预览区域`代码高亮`
* 所有选项自动记忆

## 有问题反馈
在使用中有任何问题，欢迎反馈给我，可以用以下联系方式跟我交流

* 邮件(dev.hubo#gmail.com, 把#换成@)
* QQ: 287759234
* weibo: [@草依山](http://weibo.com/ihubo)
* twitter: [@ihubo](http://twitter.com/ihubo)

## 捐助开发者
在兴趣的驱动下,写一个`免费`的东西，有欣喜，也还有汗水，希望你喜欢我的作品，同时也能支持一下。
当然，有钱捧个钱场（右上角的爱心标志，支持支付宝和PayPal捐助），没钱捧个人场，谢谢各位。

## 感激
感谢以下的项目,排名不分先后

* [mou](http://mouapp.com/)
* [ace](http://ace.ajax.org/)
* [jquery](http://jquery.com)

## 关于作者

```javascript
  var ihubo = {
    nickName  : "草依山",
    site : "http://jser.me"
  }
```
