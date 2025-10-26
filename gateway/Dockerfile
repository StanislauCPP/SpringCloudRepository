FROM openjdk:21-jdk-slim-buster
WORKDIR /app
COPY target/gateway-0.0.1-SNAPSHOT.jar ./gateway.jar
EXPOSE 9090
ENTRYPOINT ["java", "-jar", "gateway.jar", "--spring.profiles.active=cloudConfig", "--eureka.client.service-url.defaultZone=http://eureka-server:8761/eureka"]