FROM carsharing/alpine-oraclejdk8-bash
LABEL description="Spring Boot Image As rd-data"
WORKDIR /app
VOLUME /tmp
ENV LANG en_US.UTF-8

COPY rd_data_service-0.0.1-SNAPSHOT.jar rd-data.jar
RUN sh -c 'touch /rd-data.jar'

ENV JAVA_OPTS=""
EXPOSE 30728
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -jar rd-data.jar" ]
