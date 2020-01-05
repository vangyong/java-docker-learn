FROM java:8
VOLUME /tmp
ADD docker-learn.jar app.jar
RUN sh -c 'touch /app.jar'
EXPOSE 8010
ENV JAVA_OPTS=""
ENTRYPOINT [ "java", "-jar", "app.jar"]