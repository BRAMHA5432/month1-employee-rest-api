# Employee REST API (Month 1 Project)

This is a complete Spring Boot-based Employee REST API meant for a 1-month internship project.
It uses an in-memory H2 database so you can run it locally without extra setup.

## Features
- CRUD operations for Employee
- Search by name (contains)
- Pagination and sorting
- Input validation and basic error handling

## Run locally
1. Install Java 17 and Maven.
2. From project root run: `mvn spring-boot:run`
3. Open API: `http://localhost:8080/api/employees`
4. H2 console: `http://localhost:8080/h2-console` (JDBC URL: jdbc:h2:mem:employeedb)

## Example CURL
Create employee:
```bash
curl -X POST http://localhost:8080/api/employees -H "Content-Type: application/json" -d '{"name":"John","email":"john@example.com","role":"Developer","salary":50000}'
```

Get employees:
```bash
curl http://localhost:8080/api/employees
```
