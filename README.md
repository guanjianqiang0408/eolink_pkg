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
```bash
参见： https://zhuanlan.zhihu.com/p/109257078
```

安装docker
```bash
参见： https://www.cnblogs.com/Liyuting/p/17022739.html
```

使用docker安装mysql
```bash
参见: https://blog.csdn.net/weixin_43956484/article/details/116499061
```

安装java1.8
```bash
参见： https://blog.csdn.net/qq_42582489/article/details/104429639
```

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
![image](https://github.com/guanjianqiang0408/eolink_pkg/assets/103730408/e397cdfd-1438-45e5-ac92-037b7da716c5)

