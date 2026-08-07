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
