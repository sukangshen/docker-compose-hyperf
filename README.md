# docker-compose-hyperf
利用docker-compose搭建hyperf环境

##### 1.创建www目录
```
mkdir wwww

composer create-project hyperf/hyperf-skeleton 

```
##### 2.直接构建环境
```
docker-compose up -d 
```

##### 3.hyperf会依赖redis环境
```
redis.host='docker.for.mac.localhost'
```

##### 4.进入php容器内部
```
docker exec -it hyperf /bin/sh

```

##### 5.启动项目
```
cd /www/project 

composer install

php bin/hyperf.php start 
```
