# Eureka Server - GastroReview

Servidor de descubrimiento de servicios Eureka para el sistema GastroReview.

## 🚀 Tecnologías

- Java 21
- Spring Boot 3.3.3
- Spring Cloud Netflix Eureka Server
- Maven

## 📦 Compilar

```bash
mvn clean package -DskipTests
```

## ▶️ Ejecutar Localmente

```bash
mvn spring-boot:run
```

O con JAR:

```bash
java -jar target/*.jar
```

## 🌐 Puerto

Este servicio corre en el puerto **8761**.

## 🔧 Configuración para Render

### Build Command
```
mvn clean package -DskipTests
```

### Start Command
```
java -jar target/*.jar
```

### Variables de Entorno
```
JAVA_OPTS=-Xmx512m -Xms256m
PORT=8761
```

## 📊 Dashboard

Una vez desplegado, el dashboard de Eureka estará disponible en:
```
https://gastroreview-eureka.onrender.com
```

## 🔗 Microservicios Registrados

Los siguientes servicios se registrarán automáticamente:
- API Gateway
- Users Service
- Restaurants Service
- Reviews Service

## 📝 Notas

- Este servicio NO requiere base de datos
- Es el PRIMERO que debe desplegarse
- Los demás servicios necesitan su URL para registrarse

## 🔗 Enlaces

- [Spring Cloud Netflix Eureka](https://spring.io/projects/spring-cloud-netflix)
- [Documentación Spring Boot](https://spring.io/projects/spring-boot)
