# Use AdoptOpenJDK 17 JRE Alpine image (Adoptium is now Eclipse Temurin)
FROM eclipse-temurin:17-jre-alpine

# Simplify the artifact path
ARG artifact=target/spring-boot-web.jar

# Create app directory
WORKDIR /opt/app

# Copy jar to container
COPY ${artifact} app.jar

# Run Spring Boot application
ENTRYPOINT ["java", "-jar", "app.jar"]

CMD ["tail", "-f", "/dev/null"]

