# pruebaSpring

![Logo](https://raw.githubusercontent.com/spring-projects/spring-boot/main/src/main/resources/static/images/spring-logo.svg)

Proyecto de ejemplo con Spring Boot 3.3.0.

## Descripción

Esta API permite gestionar usuarios en una base de datos en memoria (HashMap). Incluye operaciones CRUD:
- Crear usuario
- Listar usuarios
- Obtener usuario por ID
- Actualizar usuario
- Eliminar usuario

## Endpoints principales

- `GET /api/users` — Lista todos los usuarios
- `GET /api/users/{id}` — Obtiene un usuario por ID
- `POST /api/users` — Crea un nuevo usuario (JSON: name, email)
- `PUT /api/users/{id}` — Actualiza un usuario existente
- `DELETE /api/users/{id}` — Elimina un usuario

## Ejemplo de petición para crear usuario

```json
{
  "name": "Juan Pérez",
  "email": "juan@example.com"
}
```

## Requisitos
- Java 17+
- Maven

## Ejecución

```sh
./mvnw spring-boot:run
```

La API estará disponible en `http://localhost:8080/api/users`
