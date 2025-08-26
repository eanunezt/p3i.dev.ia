# Proyecto P3I

P3I es una aplicación web completa diseñada para la gestión integral de estudiantes y procesos financieros. Consiste en un backend de API RESTful desarrollado con Python (FastAPI) y un frontend de administración potente y reactivo construido con React (React Admin, Material-UI).

## Características Principales

- **Gestión de Estudiantes:** Administración de perfiles de estudiantes, incluyendo su información personal y académica.
- **Módulo Financiero:**
    - Creación y gestión de **Planes de Pago** personalizados.
    - Registro y seguimiento de **Pagos** individuales asociados a los estudiantes.
- **Administración de Datos:** Gestión de datos maestros como ciudades, ubicaciones y otros catálogos.
- **Interfaz de Administración:** Un panel de control centralizado que permite a los usuarios autorizados realizar operaciones CRUD (Crear, Leer, Actualizar, Eliminar) sobre los recursos.

## Stack Tecnológico

### Backend (app.p3i.core)

- **Framework:** [FastAPI](https://fastapi.tiangolo.com/)
- **Base de Datos:** [SQLAlchemy](https://www.sqlalchemy.org/) (ORM) con [PostgreSQL](https://www.postgresql.org/)
- **Autenticación:** Tokens JWT
- **Lenguaje:** Python 3.11+

### Frontend (app-p3i)

- **Framework:** [React](https://react.dev/)
- **Framework de Admin:** [React Admin](https://marmelab.com/react-admin/)
- **Librería de Componentes:** [Material-UI (MUI)](https://mui.com/)
- **Enrutamiento:** [React Router](https://reactrouter.com/)
- **Lenguaje:** TypeScript

## Cómo Empezar

A continuación, se detallan los pasos básicos para poner en marcha el backend y el frontend.

### Iniciar el Backend

1.  **Navegar al directorio del backend:**
    ```bash
    cd app.p3i.core
    ```
2.  **Instalar dependencias (se recomienda un entorno virtual):**
    ```bash
    pip install poetry
    poetry install
    ```
3.  **Ejecutar el servidor:**
    ```bash
    poetry run start
    ```
    La API estará disponible en `http://127.0.0.1:8000`.

### Iniciar el Frontend

1.  **Navegar al directorio del frontend:**
    ```bash
    cd app-p3i
    ```
2.  **Instalar dependencias:**
    ```bash
    npm install
    ```
3.  **Ejecutar la aplicación de desarrollo:**
    ```bash
    npm run dev
    ```
    La aplicación web estará disponible en `http://localhost:5173`.
