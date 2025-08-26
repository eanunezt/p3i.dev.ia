# Estructura del Proyecto P3I

Este documento resume la estructura de los directorios principales del frontend y el backend, proporcionando un mapa rápido para el desarrollo.

## Backend (`app.p3i.core`)

El backend sigue una arquitectura en capas, con las responsabilidades claramente separadas en los siguientes directorios dentro de `src/`:

-   `src/routes/`: **Capa de Ruteo (Controladores)**. Define los endpoints de la API que reciben las peticiones HTTP y retornan las respuestas.
-   `src/services/`: **Capa de Servicios (Lógica de Negocio)**. Contiene la lógica de negocio principal, orquestando las operaciones y validaciones.
-   `src/auth/`: **Módulo de Autenticación**. Gestiona la lógica relacionada con la autenticación de usuarios y la gestión de tokens JWT.
-   `src/commons/`: **Utilidades Comunes**. Módulos y funciones compartidas a través de la aplicación, como modelos de datos, excepciones personalizadas, etc.
-   `main.py`: **Punto de Entrada**. Archivo principal que inicializa la aplicación FastAPI y sus configuraciones.

## Frontend (`app-p3i`)

El frontend está construido con React y React Admin. La estructura del directorio `src/` es la siguiente:

-   `src/admin/`: **Vistas de Recursos**. Contiene los componentes de React Admin para las operaciones CRUD (Listar, Crear, Editar, Mostrar) de cada recurso (ej. Estudiantes, Pagos).
-   `src/components/`: **Componentes Reutilizables**. Componentes de React genéricos que se utilizan en varias partes de la aplicación.
-   `src/dataprovider/`: **Proveedor de Datos**. Lógica que conecta React Admin con la API del backend. Traduce las peticiones de React Admin a peticiones HTTP para la API de FastAPI.
-   `src/layout/`: **Diseño Principal**. Componentes que definen la estructura visual de la aplicación, como el menú, la barra superior, etc.
-   `src/authProvider.ts`: **Proveedor de Autenticación**. Maneja el flujo de autenticación en el lado del cliente (login, logout, verificación de permisos).
-   `App.tsx`: **Componente Raíz**. El componente principal de React que renderiza toda la aplicación.

# Estructura de carpetas
- El archivo GEMMINI.md está dentro de p3i al mismo nivel de este archivo está app-p3i y app.p3i.core.  app-p3i/.git es el directorio del repositorio git del frontend y app.p3i.core/.git es del proyecto backend.

