
# 安装

## 连接
```shell script
redis-cli -h localhost -p 6379
redis-cli -h localhost -p 6379 -a 123456
```

## 安装卸载
```shell script
redis-server --service-install redis.windows-service.conf --loglevel verbose

redis-server --service-install

redis-server --service-install --service-name redisService1 --port 10001

redis-server --service-install --service-name redisService2 --port 10002

redis-server --service-install --service-name redisService3 --port 10003

```

## 启动
```shell script
redis-server --service-start

redis-server --service-start --service-name redisService1

redis-server --service-start --service-name redisService2

redis-server --service-start --service-name redisService3

```

## 停止
```shell script
redis-server --service-stop
```

## 卸载
```shell script
redis-server --service-uninstall

```
