FROM openjdk:17-jdk-slim-buster
WORKDIR /app
COPY target/eurekaServer-0.0.1-SNAPSHOT.jar ./eurekaServer.jar
EXPOSE 8761
ENTRYPOINT ["java", "-jar", "eurekaServer.jar", "--spring.profiles.active=cloudConfig"]