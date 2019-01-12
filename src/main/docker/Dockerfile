FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD docker-learn-1.0.0.jar docker-learn.jar
ENV TZ=Asia/Shanghai
RUN sh -c 'touch /docker-learn.jar && ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /docker-learn.jar -Xms128m -Xmx256m" ]