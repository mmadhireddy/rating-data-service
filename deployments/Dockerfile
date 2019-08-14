FROM openjdk:8-jdk-alpine
VOLUME /tmp
ADD rating-data-service-0.0.1-SNAPSHOT.jar rating-data-service.jar
RUN sh -c 'touch /movie-catalog-service.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/rating-data-service.jar"]