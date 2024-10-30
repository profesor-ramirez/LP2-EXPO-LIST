# Exposición: OAuth en .NET

## 1. Introducción a OAuth y su rol en .NET
- ¿Qué es OAuth y cómo se utiliza para autorización?
- Diferencias entre autenticación y autorización en .NET.
- Integración de OAuth en aplicaciones .NET.

## 2. Flujos de autorización en OAuth 2.0
- **Authorization Code Flow:** cómo implementarlo en aplicaciones web con .NET.
- **Implicit Flow:** para aplicaciones cliente de una sola página (SPA).
- **Client Credentials Flow:** para servicios backend.
- **Password Credentials Flow:** casos limitados y desventajas de su uso.

## 3. Autenticación basada en tokens JWT
- ¿Qué es un JSON Web Token (JWT) y cómo se utiliza en OAuth?
- Creación, validación y manejo de JWT en .NET.

## 4. Scopes y claims en OAuth
- Definición y uso de scopes en OAuth para restringir acceso a recursos.
- Uso de claims para definir permisos y roles dentro de .NET.
- Cómo definir y gestionar scopes y claims en aplicaciones .NET.

## 5. Protección de APIs en .NET con OAuth
- Configuración de políticas de autorización en APIs con `AuthorizeAttribute`.
- Cómo proteger endpoints REST en ASP.NET Core utilizando OAuth.
- Configuración de roles y permisos basados en claims en controladores API.

## 6. Refresh Tokens
- ¿Qué son y cómo funcionan los Refresh Tokens en OAuth?
- Implementación de Refresh Tokens en ASP.NET Core.
- Estrategias de seguridad para el almacenamiento y uso de Refresh Tokens.

## 7. Buenas prácticas y seguridad en OAuth
- Almacenamiento seguro de tokens en clientes y servidores.
- Medidas para evitar ataques de tipo "token hijacking" o "replay attacks".
- Uso de HTTPS y mejores prácticas de seguridad en la implementación de OAuth.

## 8. Pruebas de autenticación con Postman o herramientas similares
- Cómo probar los flujos de OAuth en .NET utilizando Postman.
- Validación de tokens y solicitudes con OAuth.