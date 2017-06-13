# Dockerfile for Java Web
为Java Web应用开发者准备的快速部署Java Web应用的镜像

参考https://gist.github.com/leapar/4e0726a56a1cbab661b3695cf9e23585

```
docker build -t leapar/tomcat:0.1 .
```


```
docker run -it --rm -p 8080:8080 leapar/tomcat:0.1
```

依赖 https://github.com/whpv/docker-bosun
