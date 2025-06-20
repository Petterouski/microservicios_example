# microservicios_example
The Microservices pattern divides an application into small independent services that communicate with each other, usually through REST APIs or messages. Each service has its own database and business logic.

This pattern is useful for large, scalable systems, where each microservice can be developed, deployed and scaled independently.
This project implements two microservices: `user_service` and `product_service`.

## Structure
- user_service**: Service to manage users.
- product_service**: Service to manage products.

## Execution
1. Install Docker and Docker Compose.
2. Navigate to the project directory.
3. Execute the command:
 ````bash
 docker-compose up --build
````

 Accede a los endpoints:
Usuarios: http://localhost:5000/users
Productos: http://localhost:5001/products


### **Construcción y Ejecución con Docker**

#### **Paso 1: Construir las imágenes**
Cuando ejecutas `docker-compose up --build`, Docker automáticamente busca el `Dockerfile` en cada carpeta especificada en el `docker-compose.yml` y construye las imágenes correspondientes.

#### **Paso 2: Verificar los contenedores**
Después de ejecutar `docker-compose up --build`, puedes verificar que ambos servicios están en ejecución usando:
```bash
docker ps