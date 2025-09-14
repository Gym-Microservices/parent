# 🏗️ Parent POM

## 📋 Descripción

POM padre para la arquitectura de microservicios del gimnasio. Centraliza la gestión de dependencias, versiones y configuraciones comunes para todos los microservicios del proyecto.

## 🎯 Propósito

- **Gestión centralizada de dependencias**: Define versiones únicas para todas las librerías
- **Configuración común**: Establece configuraciones de build compartidas
- **Estandarización**: Asegura consistencia entre todos los microservicios
- **Simplificación**: Reduce la duplicación de código en los POMs individuales

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
