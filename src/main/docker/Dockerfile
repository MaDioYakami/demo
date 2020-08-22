#指定基础镜像，在其上进行定制
FROM java:8
#作者
MAINTAINER madio maidioyakami@gmail.com
WORKDIR /ROOT
#复制上下文目录下的target/demo-1.0.0.jar 到容器里
ADD /ROOT/demo-0.0.1-SNAPSHOT.jar  /ROOT/
#指定容器启动程序及参数   <ENTRYPOINT> "<CMD>"
ENTRYPOINT ["java","-Djava.security.egd=file=/dev/./urandom","-jar","demo-0.0.1-SNAPSHOT.jar"]
CMD ["java","-version"]
