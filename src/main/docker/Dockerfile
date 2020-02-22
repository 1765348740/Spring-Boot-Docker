#镜像出处
FROM java:8
#维护者信息
MAINTAINER zlx

#将本地项目jar包拷贝到Docker容器中的位置
COPY ./demo-1.0.0.jar /app.jar
RUN bash -c 'touch /app.jar'
EXPOSE 8082
ENTRYPOINT [ "java", "-Djava.security.egd=file:/dev/./urandom", "-jar", "/app.jar" ]
