# Stage 1: Build the application using Maven and Java 1.8
FROM maven:3.8.5-openjdk-8 AS maven-build

# Set the working directory inside the container
WORKDIR /app

# Copy the pom.xml and install dependencies (this will be cached if no changes in pom.xml)
COPY . /app

# Package the application (build the JAR file)
RUN mvn clean package -DskipTests

# Stage 2: Run the application with Java 1.8
FROM openjdk:8-jre-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the built JAR file from the previous build stage
COPY --from=maven-build /app/target/*.jar app.jar

# Expose the port that your Spring Boot app will run on
EXPOSE 8080

# Command to run the JAR file
CMD ["java", "-jar", "app.jar"]