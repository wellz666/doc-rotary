doc-rotary -  比特Q
---

## 本地运行
```
sh start.sh
```
如果已安装 docker，推荐：
```shell
sh start-docker.sh
```

## 本地测试
```
sh test.sh
```

## 发布

```
heroku login
heroku container:login
heroku container:push web -a doc-rotarybit
heroku container:release web -a doc-rotarybit
heroku open -a doc-rotarybit
```

## 看日志：

```shell
heroku logs --tail -a doc-rotarybit
```

## 镜像信息：

```shell
REPOSITORY                           TAG                 IMAGE ID            CREATED             SIZE
registry.heroku.com/doc-rotary/web   latest              cc97cb425cde        4 minutes ago       1.33GB
ubuntu                               18.04               775349758637        3 weeks ago         64.2MB
```