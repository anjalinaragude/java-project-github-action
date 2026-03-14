# Use JDK 17 Alpine image
FROM eclipse-temurin:17-jdk-alpine

# Set working directory
ENV APP_HOME /usr/src/app
WORKDIR $APP_HOME

# Copy JAR built by Maven
COPY app/*.jar app.jar
# Expose port
EXPOSE 8080

# Run the Spring Boot app
ENTRYPOINT ["java", "-jar", "app.jar"]
