FROM carsharing/alpine-oraclejdk8-bash
LABEL description="Spring Boot Image As data"
WORKDIR /app
VOLUME /tmp
ENV LANG en_US.UTF-8

COPY data_service-0.0.1-SNAPSHOT.jar data.jar
RUN sh -c 'touch /data.jar'

ENV JAVA_OPTS=""
EXPOSE 30727
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -jar data.jar" ]
