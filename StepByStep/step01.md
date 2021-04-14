
## 基本概念

docker：一个应用程序。

image：封装了操作系统和特定软件的文件，这种文件只能被docker这个应用程序解析运行。

container：docker运行某个image后对应的具体实例。

repository：存储、共享image的仓库。

你可以像运行一个App一样，启动docker，然后用docker运行某特定的image文件，成功后系统里会出现一个和image相对应的container。你可以从repository下载他人制作好的image，也可以把自己制作的image上传到repository。


## 软件工程师眼中的docker

因为使用用法、关注的技术特点等方面的不同，不同的角色（软件工程师，运维工程师，分布式架构师）眼中的docker是不一样的，他们学习docker的路径也是有所不同的。从一个软件工程师的立场出发，docker能干什么呢？一个比较常见的应用场景是：在一台计算机上提供一个或多个隔离的虚拟的环境。

场景一：想学一下Linux，不需要找台机器专门装个Linux，你只需要在你计算机下载某个特定版本的Linux的image文件，然后用docker运行这个image，然后通过命令行命令进入相应container，在这个container里面，就是一个独立的Linux环境。

场景二：你想分别测试你的Python程序在不同版本的Python环境里面的运行情况。你可以在你计算机里下载不同版本的Python image文件，然后分别运行这些image文件，在运行成功后的container里面分别测试。


## docker官方的“Get Started”

docker官方文档里面有一个[Get Started](https://docs.docker.com/get-started/)系列文章，提供了一个很好的入门。它从搭建一个node js的docker开发环境为切入点，围绕着这个应用，讲解了docker相关的一些概念、原理。

1）下载运行docker，下载且运行包含了node js环境，特定node js程序和sqlite数据的image。

2）讲解如何通过repository共享image。

3）讲解如何从image里decouple数据库文件

4）讲解如何从image里decouple代码文件

5）讲解如何通过docker的network联通不同的container。

6）讲解如何通过compose来定义、运行含有多个container的app。
