
# Entry Service

Spring Boot microservice serving as the entry point of the project.

---
## Prerequisites
* Java 17+
* Gradle 8+
---

## Build and Run

From the **root of the monorepo**:

```bash
$ cd backend
$ ./gradlew build
$ java -jar entry-service/build/libs/entry-service-1.0.0.jar
```
---

## Directly Run
```bash
$ ./gradlew :entry-service:bootRun
```

## API
* `GET /ping` → returns `"pong"`
