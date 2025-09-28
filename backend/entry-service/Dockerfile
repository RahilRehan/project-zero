# Phase 1: Build
FROM gradle:8-jdk21-alpine AS build
WORKDIR /app
COPY . .
RUN gradle build 

# Phase 2: Run
FROM openjdk:21-slim
WORKDIR /app
COPY --from=build /app/build/libs/app.jar /app/app.jar
EXPOSE 8080
ENTRYPOINT ["java", "-jar", "/app/app.jar"]