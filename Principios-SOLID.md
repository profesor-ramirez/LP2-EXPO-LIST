# Exposición sobre Principios SOLID

## 1. Introducción a los Principios SOLID
- ¿Qué es SOLID?
- Historia y origen del término
- ¿Por qué es importante SOLID para un diseño de software orientado a objetos?

## 2. Principio de Responsabilidad Única (Single Responsibility Principle - SRP)
- Definición: 
- ¿Qué significa responsabilidad en el contexto de software?
- Ejemplo de una clase que no cumple el SRP.
- Beneficios de seguir SRP.

## 3. Principio de Abierto/Cerrado (Open/Closed Principle - OCP)
- Definición: 
- Ejemplo de código que no cumple con el OCP.
- Beneficios en términos de mantenimiento y escalabilidad del código.

## 4. Principio de Sustitución de Liskov (Liskov Substitution Principle - LSP)
- Definición
- Explicación del concepto de herencia y sustitución en POO.
- Relación con la herencia y el polimorfismo.
- Ejemplo de código que no cumple con el LSP.

## 5. Principio de Segregación de Interfaces (Interface Segregation Principle - ISP)
- Definición:
- Explicación del problema de las interfaces "gordas" o infladas.
- Beneficios de crear interfaces más pequeñas y específicas.

## 6. Principio de Inversión de Dependencias (Dependency Inversion Principle - DIP)
- Definición
- Diferencia entre dependencias directas y dependencias a través de abstracciones.
- Ejemplo de código que no cumple con el DIP.


## 7. Cumpliendo con el SRP
- **Basado en el siguiente código, realizar la refactorización necesaria para crear lograr que cumpla con el SRP**
```
public class User
{
    public string Name { get; set; }
    public string Email { get; set; }
    public void SaveToDatabase()
    {
        // Lógica para guardar al usuario en la base de datos
    }
    public void SendWelcomeEmail()
    {
        // Lógica para enviar un email de bienvenida
    }
}
```

## 8. Cumpliendo con el DIP
- **Basado en el siguiente código, realizar la refactorización necesaria para crear lograr que cumpla con el DIP**
```
public class Database
{
    public void SaveData(List<User> users)
    {
        // ...
    }
}

public class UserService
{
    private Database _database = new Database();
    // ...
}
```