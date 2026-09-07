# Lab 1 Arqui Soft — Backend

API REST bancaria (clientes + transferencias) construida con **Spring Boot** y **MySQL 8**.
Parte del Lab 1 del curso de Arquitectura de Software (UdeA). El frontend vive en un repo aparte:
[`lab1-arqsoft-frontend`](https://github.com/edu-delahoz/lab1-arqsoft-frontend).

## Levantar todo con Docker

```bash
docker compose up --build
```

Esto arranca:
- **MySQL 8** en el puerto `3306` (base `banco2025`, usuario/clave `root`)
- **Backend** en el puerto `8080`, esperando a que MySQL esté sano

## Desarrollo local (sin Docker)

Requiere una instancia de MySQL con la base `banco2025`. Luego:

```bash
./mvnw spring-boot:run
```

La API queda en `http://localhost:8080`.
