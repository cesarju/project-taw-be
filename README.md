# Sistema de Gestión de Estudiantes Universitarios

Este proyecto es un sistema backend para la gestión de estudiantes universitarios, desarrollado con Spring Boot. Proporciona operaciones CRUD completas para administrar la información de los estudiantes.

## Tecnologías utilizadas

- Java 21
- Lombok
- Maven

## Estructura del proyecto

```
src/
├── main/
│   ├── java/
│   │   └── com/
│   │       └── universidad/
│   │           ├── controller/       # Controladores REST
│   │           ├── dto/             # Objetos de Transferencia de Datos
│   │           ├── model/           # Entidades del dominio
│   │           ├── repository/      # Acceso a datos
│   │           ├── service/         # Lógica de negocio
│   │           └── UniversidadApplication  # Clase principal
│   └── resources/
└── test/                            # Pruebas unitarias e integración
```

## Endpoints disponibles

### Estudiantes

| Método | Endpoint                | Descripción                              |
|--------|-------------------------|------------------------------------------|
| GET    | /api/estudiantes        | Obtiene todos los estudiantes            |
| POST   | /api/estudiantes        | Crea un nuevo estudiante                 |
| PUT    | /api/estudiantes/{id}   | Actualiza un estudiante existente        |
| DELETE | /api/estudiantes/{id}   | Elimina un estudiante                    |

## Ejemplos de solicitudes

### Crear un estudiante (POST /api/estudiantes)
```json
{
    "nombre": "Ana",
    "apellido": "Torres",
    "email": "ana.torres@example.com",
    "fechaNacimiento": "2000-05-20",
    "numeroInscripcion": "S003"
}
```

### Actualizar un estudiante (PUT /api/estudiantes/{id})
```json
{
    "nombre": "Ana María",
    "apellido": "Torres",
    "email": "ana.updated@example.com",
    "fechaNacimiento": "2000-05-20",
    "numeroInscripcion": "S003"
}
```



