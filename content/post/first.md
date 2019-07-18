---
title: "First"
date: 2019-07-11T20:47:39+08:00
draft: true
---


# 一些知识的记录

## [点赞请来这里 ʘᴗʘ](https://git.antiy.org.cn/xingjichen/blog/issues/1)

[Markdown基本语法](https://www.jianshu.com/p/191d1e21f7ed)

[Docker中容器的备份、恢复和迁移](https://www.cnblogs.com/boshen-hzb/p/6373549.html)

```shell
创建快照
docker commit -p 30b8f18f20b4 container-backup
另存为文件
docker save -o ~/container-backup.tar container-backup
重新载入快照
docker load -i ~/container-backup.tar
```

[删除docker镜像并释放空间](https://www.zhihu.com/question/45081896)

```shell
docker rm $(docker ps -a -q)
docker rmi $(docker images -q)
docker volume rm $(docker volume ls |awk '{print $2}')
rm -rf ~/Library/Containers/com.docker.docker/Data/*
```
