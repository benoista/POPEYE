FROM maven:3.9.6-eclipse-temurin-21-alpine AS builder

# Defined the working directory
WORKDIR /app

# Copy the files
COPY . .

RUN mvn dependency:resolve

RUN mvn package

FROM eclipse-temurin:21-jre-alpine

WORKDIR /app

COPY --from=builder /app/target/*.jar .



# Start App
CMD ["java", "-jar", "worker-jar-with-dependencies.jar"]



