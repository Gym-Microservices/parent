# 🏗️ Parent POM

## 📋 Descripción

POM padre para la arquitectura de microservicios del gimnasio. Centraliza la gestión de dependencias, versiones y configuraciones comunes para todos los microservicios del proyecto.

## 🎯 Propósito

- **Gestión centralizada de dependencias**: Define versiones únicas para todas las librerías
- **Configuración común**: Establece configuraciones de build compartidas
- **Estandarización**: Asegura consistencia entre todos los microservicios
- **Simplificación**: Reduce la duplicación de código en los POMs individuales

## 📦 Dependencias Gestionadas

### 🌸 Spring Framework

- **Spring Boot**: 3.5.4
- **Spring Cloud**: 2025.0.0
- **Spring Boot Starter Parent** como POM padre base

### 🗄️ Base de Datos

- **H2 Database**: 2.2.224 (base de datos en memoria para desarrollo)

### 🛠️ Herramientas de Desarrollo

- **Lombok**: 1.18.30 (generación automática de código)
- **Spring Boot DevTools**: Hot reload para desarrollo
- **Jackson JSR310**: Soporte para fechas/tiempo de Java 8+

### 🧪 Testing

- **Spring Boot Starter Test**: Framework completo de testing

## ⚙️ Configuración

### ☕ Java

- **Versión**: Java 17
- **Encoding**: UTF-8
- **Maven Compiler**: 3.11.0

### 📤 Distribución

- **Repositorio**: GitHub Packages
- **Grupo**: com.gym
- **Artifact**: gym-microservices-parent

## 🔗 Uso

Los microservicios heredan de este POM padre agregando la siguiente configuración:

```xml
<parent>
    <groupId>com.gym</groupId>
    <artifactId>gym-microservices-parent</artifactId>
    <version>0.0.1-SNAPSHOT</version>
    <relativePath>../parent</relativePath>
</parent>
```

## 🛠️ Tecnologías

- Maven Multi-Module Project
- Spring Boot
- Spring Cloud
- GitHub Packages
