# Apache加载PHP模块

## 1：在Apache的主配置文件中加载对应的PHP提供的模块

``

* LoadModule php7_module PHP所提供的模块链接所在的路径
** Apache主配置文件所在地址 D:\Server\Apache24\conf/httpd.config
*** 在httpd.config文件内加入 LoadModule php7_module 'PHP所提供的模块链接所在的路径'
**** PHP_study\3-配置Apache加载PHP模块\images\config中配置php.png
``

## 2：Apache分配工作给PHP模块：如果是PHP代码就交给PHP处理（文件后缀名判断是否为.php）

``

* AddType application/x-httpd-php .php
** PHP_study\3-配置Apache加载PHP模块\images\Apache分配给PHP.png

``

## 3：将PHP配置文件加载到Apache配置文件中：共同生效

``

* 3.1：在Apache中指定PHP配置文件所在路径
** PHPIniDir php.ini所在路径
*** PHP_study\3-配置Apache加载PHP模块\images\在Apache中指定PHP配置文件所在路径.png

* 3.2：php.ini文件默认不存在，是以development 和 production 格式存在，需要格式化
** 将php文件内的php.ini-development文件重名为php.ini
*** PHP_study\3-配置Apache加载PHP模块\images\php.ini.png

``

### 说明：PHP配置文件已经加入到Apache的配置项中，意味着 php.ini 的修改需要Apache重启才会生效
