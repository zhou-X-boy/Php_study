# PHP连接MySQL数据库

## PHP本身不具备操作MySQL数据库的能力，需要借助PHP操作MySQL的扩展来实现

··

* 1：PHP加载MySQL扩展：`php.ini`文件中
**PHP_study\6-PHP加载MySQL扩展\images\1-PHP配置MySQL加载扩展.png

*** 这里是php7，已经将mysql的拓展移出，所以使用`pdo_mysql`

****PHP_study\6-PHP加载MySQL扩展\images\2-1php7加载pdo_mysql.png

****PHP_study\6-PHP加载MySQL扩展\images\2-2php7加载pdo_mysql.png

**** PHP_study\6-PHP加载MySQL扩展\images\2-3php.ini文件内的改变.png

**** PHP_study\6-PHP加载MySQL扩展\images\2-4php.ini文件内的改变.png

* 2：PHP中所有的扩展都在ext文件夹中，需要制定扩展所在的路径：extension_dir = "D:\Server\php7\ext"
** PHP_study\6-PHP加载MySQL扩展\images\2-4php.ini文件内的改变.png

* 3；PHP已经被Apache加载，所以需要重启服务器才会生效
··
