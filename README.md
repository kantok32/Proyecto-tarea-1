# Task Manager App

## Descripción
La aplicación **Task Manager App** es una herramienta de gestión de tareas que permite a los usuarios crear, actualizar, completar, eliminar y gestionar tareas a través de una interfaz gráfica en Python. Utiliza una base de datos **SQLite** para almacenar las tareas y **Pandas** para mostrar las tareas en formato tabular.

Además, la aplicación permite exportar e importar tareas en formato **JSON**.

## Funcionalidades
- **Agregar tareas**: Crear nuevas tareas con título y descripción.
- **Marcar tareas como completadas**: Cambiar el estado de una tarea a "Completada".
- **Eliminar tareas**: Eliminar tareas de la base de datos.
- **Exportar tareas**: Exportar todas las tareas a un archivo **JSON**.
- **Importar tareas**: Cargar tareas desde un archivo **JSON**.

## Requisitos
- **Python 3.6 o superior**.
- **Bibliotecas de Python**: Las bibliotecas necesarias son:
  - **SQLAlchemy**: Para gestionar la base de datos.
  - **Pandas**: Para mostrar las tareas en formato tabular.
  - **Tkinter**: Para crear la interfaz gráfica de la aplicación.

## Instalación

### 1. Clonar el repositorio
Clona este repositorio en tu máquina local.

```bash
git clone https://github.com/tu-usuario/task-manager-app.git
cd task-manager-app
