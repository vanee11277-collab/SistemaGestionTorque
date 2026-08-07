# SistemaGestionTorque

## Proyecto Integrador Tecmilenio

### Empresa
Polaris Industries

### Área
Torque

### Descripción

Sistema de Gestión y Análisis de Torque para el monitoreo de herramientas Atlas Copco y consulta de información proveniente de ToolsNet.

El sistema permitirá:

- Consulta por VIN
- Consulta de herramientas
- Consulta de controladores
- Consulta de eventos
- Generación de reportes
- Administración de alertas
## Problema Identificado

Actualmente el área de Torque utiliza la plataforma Atlas Copco ToolsNet para almacenar información relacionada con resultados de torque, VIN de las unidades, eventos de herramientas, estados de controladores y datos históricos. Sin embargo, cuando se requiere investigar una falla, analizar tendencias o localizar información específica, es necesario consultar diferentes reportes y fuentes de información. Debido al volumen de datos generado diariamente, el análisis puede consumir tiempo considerable y dificultar la identificación rápida de problemas recurrentes.

## Solución Propuesta

Desarrollar un Sistema de Gestión y Análisis de Torque que permita centralizar consultas, realizar búsquedas por VIN, herramienta o controlador, generar reportes de manera rápida e identificar tendencias y alertas relevantes para el personal de Torque.

Las principales funcionalidades incluyen:

- Consulta por VIN.
- Consulta de herramientas.
- Consulta de controladores.
- Consulta de eventos.
- Historial de torques.
- Generación de reportes.
- Administración de usuarios.
- Gestión de alertas.
- ## Arquitectura

```text
                Usuario
                    │
                    ▼
          Interfaz Web del Sistema
                    │
                    ▼
     Sistema de Gestión y Análisis
                 de Torque
                    │
     ┌──────────────┼──────────────┐
     ▼              ▼              ▼
 Herramientas   Controladores    Eventos
     │              │              │
     └──────────────┼──────────────┘
                    ▼
             Datos de Torque
                    │
                    ▼
              Base de Datos
                    │
                    ▼
          Alertas y Reportes
### Tecnologías

- Java
- Git
- GitHub

### Autor

Vanessa Yamileth Aguado Rangel
## Tabla de Contenidos

- Descripción
- Problema Identificado
- Solución Propuesta
- Arquitectura
- Requerimientos
- Instalación
- Configuración
- Uso
- Contribución
- Roadmap

## Requerimientos

### Servidor de Aplicación

- Apache Tomcat 10

### Servidor Web

- Apache Tomcat

### Base de Datos

- MySQL 8.0

### Lenguaje de Programación

- Java 17

### Control de Versiones

- Git
- GitHub

### Integración Continua

- GitHub Actions

### Paquetes Adicionales

- Maven
- JUnit
- Spring Boot
- Spring Data JPA
- MySQL Connector/J

## Instalación

### Instalación del ambiente de desarrollo

1. Instalar Java 17.
2. Instalar Git.
3. Instalar Apache Tomcat 10.
4. Instalar MySQL 8.0.
5. Clonar el repositorio:

```bash
git clone https://github.com/vanee11277-collab/SistemaGestionTorque.git
```

### Ejecutar pruebas manualmente

```bash
mvn test
```

### Implementación local

```bash
java -jar SistemaGestionTorque.jar
```

## Configuración

### Configuración del producto

Archivo:

```text
application.properties
```

Ejemplo:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/torque
spring.datasource.username=root
spring.datasource.password=1234

server.port=8080
```

### Configuración de requerimientos

- Java 17
- Apache Tomcat 10
- MySQL 8.0
- Maven
- Git

## Uso

### Usuario final

El usuario final podrá:

- Consultar información por VIN.
- Consultar eventos.
- Consultar historial de torque.
- Generar reportes.
- Visualizar alertas.

### Usuario Administrador

El administrador podrá:

- Crear usuarios.
- Modificar usuarios.
- Gestionar permisos.
- Registrar herramientas.
- Administrar controladores.
- Configurar el sistema.

## Contribución

### Clonar repositorio

```bash
git clone https://github.com/vanee11277-collab/SistemaGestionTorque.git
```

### Crear branch

```bash
git checkout -b feature-nueva-funcionalidad
```

### Realizar cambios

```bash
git add .
git commit -m "Nueva funcionalidad"
```

### Enviar cambios

```bash
git push origin feature-nueva-funcionalidad
```

### Pull Request

1. Crear Pull Request hacia develop.
2. Esperar revisión.
3. Aprobar cambios.
4. Realizar merge.

## Roadmap

### Versión Beta

- Inicio de sesión.
- Gestión de usuarios.
- Gestión de herramientas.
- Gestión de controladores.
- Consulta por VIN.
- Consulta de eventos.

### Versión GA

- Historial de torques.
- Sistema de alertas.
- Generación de reportes.
- Seguridad y auditoría.
- Pruebas finales.

### Futuras versiones

- Aplicación móvil.
- Integración con Power BI.
- Inteligencia artificial para predicción de fallas.
- Integración en tiempo real con ToolsNet.
- Notificaciones por correo electrónico.

