
# Entry Service

Spring Boot microservice serving as the entry point of the project.

---
## Prerequisites
* Java 21+
* Gradle 8+
---

## Build and Run

From the **root of the monorepo**:

```bash
$ cd backend/entry-service
$ docker build -t entry-service .
$ docker run -p 8080:8080 entry-service:latest
```
---

## API
* `GET /ping` → returns `"pong"`
