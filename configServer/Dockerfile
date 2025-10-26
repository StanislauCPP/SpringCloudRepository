FROM openjdk:21-jdk-slim-buster
WORKDIR /app
COPY target/configServer-0.0.1-SNAPSHOT.jar ./configServer.jar
COPY config/ ./config/
EXPOSE 8888
ENTRYPOINT ["java", "-jar", "configServer.jar", "--spring.profiles.active=standalone,native"]