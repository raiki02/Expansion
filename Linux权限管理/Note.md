root用户#和普通用户$

su user_name/root转换

用户对文件的权限：用户对文件的角色（u，g，o）+文件赋予角色的权限

键入ll查看文件属性

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/3d26a2e426175b7138be3b15b9a5900e.png)

文件类型：

d：文件夹

-： 普通文件

l： 软连接(快捷)

**b： 块设备(硬盘，光驱)**

p： 管道

**c： 字符设备(屏幕串口设备)**

**s： 套接口**

访问权限：

r： 可读

w： 可写

x： 可执行

-： 无权限

前三：user； 中三：group； 后三： others

值表示方法：（wrx）

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/036d70d9f5fa76e30860289bf5b1303a.png)

修改权限：

chmod [选项] 用户+/-/=某项权限 文件名

+：添加； -：取消； =： 赋予

eg：chmod g-w testf

-R选项： 递归修改文件权限

可以使用3个八进制值表示方法修改权限（分别是ugo）

eg： chmod 666 testf

