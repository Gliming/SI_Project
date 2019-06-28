FROM carsharing/alpine-oraclejdk8-bash
LABEL description="Spring Boot Image As zipkin"

ENV LANG en_US.UTF-8

COPY zipkin_server-0.0.1-SNAPSHOT.jar zipkin.jar
RUN sh -c 'touch /zipkin.jar'

ENV JAVA_OPTS=""
EXPOSE 9411
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -jar zipkin.jar" ]
