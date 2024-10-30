nginx

## **反向代理**

​	proxy(代理)： 中介服务器，在C，S之间通信

​	功能：藏ip，限制访问，缓存减压，负载均衡(分配到多个S)，安全层

![img](https://i-blog.csdnimg.cn/blog_migrate/056f43dba2b0feddcb46cbc4ecaa4d23.png#pic_center)

正：S不了解谁来了

反：C不知道谁做了

透明代理？

## **SSL证书，http->https**

SSL证书绑定特定域名。

配置https服务，必须有SSL证书。

找对应的服务器商。