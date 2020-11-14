# 1：服务器进程，运行之后服务器才能工作

## 2：用来查看Apache具有哪些功能以及配置文件是否有错

``
httpd 或者 httpd.exe(cmd进入文件所在目录)
``

### 2.1：查看使用的模块

``
** httpd.exe -M

** PHP_study\1-安装Apache\images\查看使用模块.png

``

### 2.2：验证配置文件是否有效

``
** httpd -t

** PHP_study\1-安装Apache\images\验证配置文件是否有效.png
``
