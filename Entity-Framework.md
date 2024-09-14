# Exposición sobre Entity Framework

## 1. Introducción a Entity Framework
- ¿Qué son los ORM (Object-Relational Mapping)?
- ¿Qué es Entity Framework?
- Ventajas de usar Entity Framework en comparación con ADO.NET y otras tecnologías.

## 2. Modelos de Desarrollo en Entity Framework
- Database-First: 
- Code-First:
- Model-First: 

## 3. Configuración de Entity Framework
- Instalación de EF en un proyecto .NET (uso de `NuGet`).
- Configuración en el archivo `appsettings.json` para establecer la cadena de conexión a la base de datos.
- Uso del `DbContext` como punto de entrada para interactuar con la base de datos.

## 4. Definición del Modelo de Datos
- Como se define un modelo de datos, es decir, la creación de clases y propiedades que representan las tablas y columnas en la base de datos.
- Atributos y convenciones para mapear clases y propiedades a tablas y columnas.

## 5. Migrations
- ¿Qué son las migraciones en EF?
- Como se Crean y aplican las migraciones.
- Diferencia entre migraciones automáticas vs. manuales.

## 6. Consultas en EF (LINQ)
- Uso de **LINQ** (Language-Integrated Query) para realizar consultas.
- Consultas básicas: `Where`, `Select`, `OrderBy`.


## 7. Database First con EF 
- **Basado en el siguiente script SQL, realizar los procesos necesarios para crear el modelo con Entity Framework**
```
-- Crear la base de datos
CREATE DATABASE TiendaEnLinea;
GO

USE TiendaEnLinea;
GO

-- Crear las tablas
CREATE TABLE Productos (
    Id INT IDENTITY(1,1) PRIMARY KEY,
    Nombre VARCHAR(100) NOT NULL,
    Descripcion TEXT,
    Precio DECIMAL(10,2) NOT NULL,
    Stock INT NOT NULL
);
```

## 8. Code First con EF 
- **Basado en la siguiente clase, realizar los procesos necesarios para crear realizar la migración a la base de datos con Entity Framework**
```
public class Post
{
    public int Id { get; set; } // Clave primaria autoincremental
    public string Titulo { get; set; }
    public string Contenido { get; set; }
    public DateTime FechaPublicacion { get; set; }
    public string Autor { get; set; }
    public int CategoriaId { get; set; }
}
```