# Drivers arquitectónicos

## Descripción

Los drivers arquitectónicos son los requisitos y restricciones que tienen mayor influencia sobre las decisiones de diseño de la arquitectura del marketplace.

## Drivers arquitectónicos

### DA01 - Escalabilidad

El sistema debe soportar un incremento importante de usuarios y solicitudes durante campañas comerciales y promociones.

**Relacionado con:** AC03 - Escalabilidad.

**Impacto arquitectónico:** La arquitectura debe permitir ampliar la capacidad del sistema mediante mecanismos de escalamiento.

### DA02 - Rendimiento

El sistema debe proporcionar tiempos de respuesta adecuados ante una cantidad elevada de usuarios concurrentes.

**Relacionado con:** AC01 - Rendimiento.

**Impacto arquitectónico:** Se debe considerar una comunicación eficiente entre componentes, procesamiento adecuado y un almacenamiento que permita atender múltiples solicitudes.

### DA03 - Seguridad

El sistema debe proteger la información de los usuarios y de las compras frente a accesos no autorizados.

**Relacionado con:** AC04 - Seguridad.

**Impacto arquitectónico:** Se deben considerar mecanismos de autenticación, autorización y protección de los datos.

### DA04 - Integración con servicios externos

El sistema debe integrarse con una pasarela de pago externa para procesar las transacciones de los clientes.

**Relacionado con:** RC04 - Pasarela de pago externa.

**Impacto arquitectónico:** La arquitectura debe permitir la comunicación e integración con servicios externos mediante interfaces bien definidas.

### DA05 - API REST

El sistema debe utilizar una API REST para la comunicación entre la aplicación web y los servicios del sistema.

**Relacionado con:** RC03 - API REST.

**Impacto arquitectónico:** La arquitectura debe separar la presentación de la lógica de negocio y permitir una comunicación mediante servicios REST.

## Resumen

| ID   | Driver              | Relación | Impacto arquitectónico                                         |
| ---- | ------------------- | -------- | -------------------------------------------------------------- |
| DA01 | Escalabilidad       | AC03     | Permitir ampliar la capacidad del sistema.                     |
| DA02 | Rendimiento         | AC01     | Atender múltiples solicitudes eficientemente.                  |
| DA03 | Seguridad           | AC04     | Implementar autenticación, autorización y protección de datos. |
| DA04 | Integración externa | RC04     | Permitir integración con servicios externos.                   |
| DA05 | API REST            | RC03     | Separar presentación y lógica mediante servicios REST.         |
