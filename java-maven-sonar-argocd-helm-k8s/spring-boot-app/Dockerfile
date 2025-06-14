# Use AdoptOpenJDK 17 JRE Alpine image (Adoptium is now Eclipse Temurin)
FROM eclipse-temurin:17-jre-alpine

# Simply the artifact path
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

# This should not be changed
ENTRYPOINT ["java","-jar","app.jar"]
