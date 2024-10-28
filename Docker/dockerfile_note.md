**FROM起手: 设置基础镜像，后续的操作都是基于它的**

​	`FROM ubuntu:20.04`

**RUN： 后跟shell格式或者exec格式，相当于执行命令行命令**

​	`RUN apt-get update && apt-get install -y curl`

注：每RUN一次都会搭建一层镜像，可以用一个RUN执行多个命令，每个命令用&&连接

**ENV：环境变量**

​	`ENV NODE_ENV=production`

​	` ENV PORT=3000`

**EXPOSE：运行时监听端口**

​	`EXPOSE <port> [<port>/<protocol>...]`

**CMD：启动时执行的命令，以最后一个CMD为准生效，exec，shell两种格式**

​	`CMD ["echo", " hello, world! "]`

​	`CMD echo " hello world! " `

注：docker run指定命令和参数时当作CMD处理

 

