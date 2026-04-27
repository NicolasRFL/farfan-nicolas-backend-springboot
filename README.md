## Descripción

Proyecto de backend desarrollado con Java Spring Boot, diseñado para ofrecer una API REST escalable y lista para desplegar en contenedores Docker. Ideal para aplicaciones empresariales que requieren una configuración rápida y un entorno reproducible.

## Tecnologías

- Java 17+
- Spring Boot
- Spring Web
- Spring Data JPA
- Docker
- Maven o Gradle
- Base de datos relacional MySQL

## Requisitos previos

- Docker instalado y en ejecución
- Docker Compose
- Acceso a la terminal o línea de comandos

## Cómo ejecutar con Docker
Desde la carpeta donde se encuentra el docker-compose.yml.
1. Construir la imagen Docker:
    ```
    docker compose build
    ```

2. Ejecutar el contenedor:
    ```
    docker compose up -d
    ```

3. Verificar que la aplicación esté en ejecución:
    ```
    docker ps
    ```

## Endpoints principales

- `GET /api/articulos` – Obtener la lista de artículos
- `GET /api/articulos/{id}` – Obtener un recurso por su identificador
- `POST /api/articulos` – Crear un nuevo recurso
- `PUT /api/articulo/{id}` – Actualizar un recurso existente
- `DELETE /api/articulos/{id}` – Eliminar un recurso

## Stack tecnológico

- Java 17+
- Spring Boot
- Spring Data JPA
- MySQL / PostgreSQL
- Docker
- Docker Compose
- Maven o Gradle

## Instalación y ejecución con Docker Compose

1. Clona el repositorio:
    ```bash
    git clone https://github.com/NicolasRFL/farfan-nicolas-backend-springboot
    cd entrega-farfan-nicolas
    ```

2. Construye y levanta los servicios con Docker Compose:
    ```bash
    cd carrito
    docker compose up --build
    ```

3. Verifica que los contenedores estén en ejecución:
    ```bash
    docker compose ps
    ```

4. Accede a la API en:
    - `http://localhost:8080`

## Endpoints principales

La API REST ofrece operaciones CRUD sobre la entidad principal. Entre las rutas más relevantes están:
- `GET /api/entidades`
- `GET /api/entidades/{id}`
- `POST /api/entidades`
- `PUT /api/entidades/{id}`
- `DELETE /api/entidades/{id}`

## Estructura del proyecto

- `src/main/java/`
  - `com.talento.controller/` – controladores REST
  - `com.talento.service/` – lógica de negocio
  - `com.talento.repository/` – acceso a datos JPA
  - `com.talento.model/` – entidades y modelos
  - `com.talento.config/` – configuración de la aplicación

- `src/main/resources/`
  - `application.properties` – configuración de Spring Boot

- `Dockerfile`
- `docker-compose.yml`
- `pom.xml`

Con esta estructura, el proyecto está preparado para ejecutarse en contenedores y conectarse a una base de datos relacional compatible como MySQL o PostgreSQL.
