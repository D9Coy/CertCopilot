# Library App

## Descripción

**Library App** es una aplicación de consola para la gestión de una biblioteca. Permite administrar usuarios (patrons), préstamos, y recursos de la biblioteca, siguiendo una arquitectura por capas que separa la lógica de negocio, la infraestructura y la interfaz de usuario. Incluye pruebas unitarias para garantizar la calidad del software.

## Estructura del Proyecto

- AccelerateDevGitHubCopilot.sln
- README.md
- src/
  - Library.ApplicationCore/
    - Library.ApplicationCore.csproj
    - Entities/
    - Enums/
    - Interfaces/
    - Services/
  - Library.Console/
    - appSettings.json
    - CommonActions.cs
    - ConsoleApp.cs
    - ConsoleState.cs
    - Library.Console.csproj
    - Program.cs
    - Json/
      - Patrons.json
  - Library.Infrastructure/
    - Library.Infrastructure.csproj
    - Data/
- tests/
  - UnitTests/
    - LoanFactory.cs
    - ...

## Clases e Interfaces Clave

- **Entities/**  
  Contiene las entidades principales del dominio, como usuarios, préstamos, libros, etc.

- **Enums/**  
  Define enumeraciones utilizadas en la lógica de negocio.

- **Interfaces/**  
  Define contratos para servicios y repositorios, facilitando la inyección de dependencias y pruebas.

- **Services/**  
  Implementa la lógica de negocio principal y los servicios de la aplicación.

- **ConsoleApp.cs**  
  Clase principal para la ejecución de la aplicación de consola.

- **CommonActions.cs**  
  Acciones comunes reutilizables en la consola.

- **ConsoleState.cs**  
  Maneja el estado de la aplicación de consola.

- **Patrons.json**  
  Archivo de datos con la información de los usuarios de la biblioteca.

## Uso

1. Clona el repositorio.
2. Abre la solución `AccelerateDevGitHubCopilot.sln` en Visual Studio.
3. Restaura los paquetes NuGet si es necesario.
4. Establece `Library.Console` como proyecto de inicio.
5. Ejecuta la aplicación para interactuar con la biblioteca desde la consola.
6. Para ejecutar las pruebas unitarias, selecciona el proyecto `UnitTests` y ejecuta las pruebas desde el Test Explorer.

## Licencia

Este proyecto está licenciado bajo los términos de la licencia MIT.

