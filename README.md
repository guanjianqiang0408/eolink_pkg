## eolink 目录说明

config/setting.properties   eolinker配置文件

eolinker_os.sql    eolinker初始化数据文件

eolinker_os-4.0.jar  eolinker运行jar包



## 部署依赖说明

docker 24.0.2

mysql 5.7

java 1.8

nginx 1.14.1



## 部署说明

安装nginx

安装docker

使用docker安装mysql
```bash
参见: https://blog.csdn.net/weixin_43956484/article/details/116499061
```

安装java1.8

创建mysql数据库

```sql
create database enlinker_os default charset utf8
```

执行eolinker_os.sql初始化数据库

启动eolinker服务

```bash
nohup java -jar eolinker_os-4.0.jar &
```

访问测试：

http://ip:port/eolinker_os/index.html

![image-20230829144035442](C:\Users\v_gjqguan\AppData\Roaming\Typora\typora-user-images\image-20230829144035442.png)
