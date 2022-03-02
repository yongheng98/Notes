# docker



```
docker pull image:版本
docker pull mysql:5.7.30 

docker images // 看本地有没有下载下来

docker run -itd --name mysql-test -p 3306:3306 -e MYSQL_ROOT_PASSWORD=123456 mysql:5.7.30

docker ps // 查看正在运行的docker app

C:\Users\admin>docker exec -it mysql-test /bin/bash
root@988e87d4fe5c:/# mysql -h localhost -uroot -p123456
或者root@988e87d4fe5c:/# mysql -uroot -p123456
>mysql //代表进入服务，成功


docker kill mysql-test // 结束docker进程


也可以直接，docker desktop -> containers/apps -> cli
># mysql -uroot -p123456
```

