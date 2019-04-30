FROM openjdk:7-jre-slim
MAINTAINER xuxueli

ENV PARAMS=""

ENV TZ=PRC
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

# ADD target/xxl-job-admin-*.jar /app.jar
ADD http://dockers-files.oss-cn-hangzhou.aliyuncs.com/xxl-job/xxl-job-admin-2.1.0-SNAPSHOT.jar /app.jar

ENTRYPOINT ["sh","-c","java -jar /app.jar $PARAMS"]
