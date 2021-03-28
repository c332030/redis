
# 数据类型

## string
一个键最大能存储512MB

## hash
类似于 map，每个 hash 可以存储 232 -1 键值对（40多亿）。

适合存储对象

```shell script
HMSET myhash field1 "Hello" field2 "World"

HGET myhash field1
HGET myhash field2
```

## set
集合中最大的成员数为 232 - 1(4294967295, 每个集合可存储40多亿个成员)。

```shell script
sadd runoob redis
# (integer) 1

sadd runoob mongodb
# (integer) 1

sadd runoob rabitmq
# (integer) 1

sadd runoob rabitmq
# (integer) 0

smembers runoob
# 1) "redis"
# 2) "rabitmq"
# 3) "mongodb"

```
