# Use Java 17
FROM eclipse-temurin:17-jdk-alpine

# App directory
WORKDIR /app

# Copy project
COPY . .

# Build the app
RUN ./mvnw clean package -DskipTests

# Expose Spring Boot port
EXPOSE 8080

# Run the app
CMD ["java", "-jar", "target/*.jar"]
