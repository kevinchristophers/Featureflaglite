# FeatureFlagLite — Simple Feature Flag and Configuration Management Service

> **College Assessment Project (Question 75)**  
> **A robust, production-grade Spring Boot & MySQL feature flagging microservice with environment-specific overrides, deterministic percentage rollout, and full audit change logging.**

---

## 📌 1. Project Title & Problem Statement

### Problem Statement
In modern software engineering, deploying new features directly to production presents risks. Traditional applications require code commits, rebuilds, and full redeployments merely to toggle a feature ON or OFF or to change configuration across staging environments.

### Solution: FeatureFlagLite
**FeatureFlagLite** decouples feature release from code deployment. It provides a centralized, database-backed REST service where features can be dynamically controlled per environment (`DEV`, `TEST`, `PROD`) and rolled out gradually (0% to 100%) to target user subsets using deterministic hashing—without restarting or redeploying any services.

---

## 🛠️ Technology Stack
- Java 17
- Spring Boot 3.4.3
- Spring Web / REST
- Spring Data JPA & Hibernate
- MySQL 8.0+
- Jakarta Bean Validation
- Lombok
- MockMvc / JUnit 5

---

## 📁 Key Documentation Links
- [POSTMAN_GUIDE.md](file:///c:/Users/asus/Downloads/featureflaglite/featureflaglite/POSTMAN_GUIDE.md): 17-step testing and demonstration sequence.
- [DATABASE_SETUP.md](file:///c:/Users/asus/Downloads/featureflaglite/featureflaglite/DATABASE_SETUP.md): MySQL configuration, schemas, and queries.
- [postman_collection.json](file:///c:/Users/asus/Downloads/featureflaglite/featureflaglite/postman_collection.json): One-click Postman collection import.

---

## 🚀 How to Run
```bash
cd featureflaglite
mvn clean spring-boot:run
```

To run all automated test cases:
```bash
mvn clean test
```
