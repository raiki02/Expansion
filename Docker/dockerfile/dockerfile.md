#### 1.base

**FROM起手: 设置基础镜像，后续的操作都是基于它的**

​	`FROM ubuntu:20.04`



**RUN： 后跟shell格式或者exec格式，相当于执行命令行命令** 镜像构建时

​	`RUN apt-get update && apt-get install -y curl`

注：每RUN一次都会搭建一层镜像，可以用一个RUN执行多个命令，每个命令用&&连接



**CMD：启动时执行的命令，以最后一个CMD为准生效，exec，shell两种格式** 容器运行时，结束生命周期

​	`CMD ["echo", " hello, world! "]`

​	`CMD echo " hello world! " `

注：docker run指定命令和参数时当作CMD处理



**ENV：环境变量**

​	`ENV NODE_ENV=production`

​	` ENV PORT=3000` 



**ARG：构建参数** 



**EXPOSE：运行时监听端口**

​	`EXPOSE <port> [<port>/<protocol>...]`



**WORKDIR：指令在这里执行**



**COPY：从[宿主机]拷贝到[镜像]**



**ADD：类似COPY但是可以添加URL**



**VOLUME ： 映射容器文件**



**ONBUILD：基于基镜像的镜像(继承) 的操作**



**构建：docker build -t container_name(: tag) .**

**运行：docker run container_name(:tag)**

#### 2.diff

**ADD & COPY**

能C就C

**CMD & ENTRYPOINT**

![image-20241031142159264](C:\Users\49071\AppData\Roaming\Typora\typora-user-images\image-20241031142159264.png)

ET先行 JSON拼接

**ARG & ENV**

有效期：E全局，A构建
