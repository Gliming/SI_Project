FROM carsharing/alpine-oraclejdk8-bash
LABEL description="Spring Boot Image As eureka"

ENV LANG en_US.UTF-8

COPY eureka_server-0.0.1-SNAPSHOT.jar eureka.jar
RUN sh -c 'touch /eureka.jar'

ENV JAVA_OPTS=""
EXPOSE 8761
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -jar eureka.jar" ]
