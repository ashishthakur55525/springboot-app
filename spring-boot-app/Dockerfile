# You can change this base image to anything else
# But make sure to use the correct version of Java
FROM arm64v8/eclipse-temurin:21-jre

# FROM alpine:3.21.0

# FROM alpine/java:22-jdk

# FROM adoptopenjdk/openjdk11:x86_64-debian-jre-11.0.25_9
# Simply the artifact path
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

# This should not be changed
ENTRYPOINT ["java","-jar","app.jar"]
