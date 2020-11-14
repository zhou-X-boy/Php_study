# MySQL访问流程

* MySql是一个C/S架构的软件，需要通过客户端来访问服务端（MySQL也提供了其他模式的访问，通过一些插件扩展来充当客户端）

## 1：启动MySQL客户端：运行mysql.exe，该软件本身可以通过CMD控制台运行

``

* 本身的客户端：mysql.exe
** PHP_study\5-MySql的访问流程\images\1-本身的客户端mysql.exe.png

* MySQL通过CMD运行
** PHP_study\5-MySql的访问流程\images\2-cmd运行.png

``

## 2：MySQL客户端访问服务端需要进行寻找匹配：连接认证

``

* 连接：IP和端口确认，如果是本地都可以省略
**-h主机地址-->-hlocalhost(可以是IP地址)
** -P端口--> -P3306

* 认证：通过用户名和密码进入服务器
**-u用户名 --> -uroot(不可以省略（匿名用户除外）)
** -p密码 --> -proot

*** PHP_study\5-MySql的访问流程\images\3-连接认证.png
``

## 3：退出命令：\q

· PHP_study\5-MySql的访问流程\images\4-退出命令.png

### 注意：通常连接认证的时候密码不建议明文，可以在输入 -p 后回车，系统会在次让输入密码，这个时候就是密文

. PHP_study\5-MySql的访问流程\images\5-输入密码密文.png
