Descripción
La aplicación Task Manager App es una herramienta de gestión de tareas que permite a los usuarios crear, actualizar, completar, eliminar y gestionar tareas a través de una interfaz gráfica en Python. Utiliza una base de datos SQLite para almacenar las tareas y Pandas para mostrar las tareas en formato tabular.

Además, la aplicación permite exportar e importar tareas en formato JSON.

Funcionalidades
Agregar tareas: Crear nuevas tareas con título y descripción.
Marcar tareas como completadas: Cambiar el estado de una tarea a "Completada".
Eliminar tareas: Eliminar tareas de la base de datos.
Exportar tareas: Exportar todas las tareas a un archivo JSON.
Importar tareas: Cargar tareas desde un archivo JSON.
Requisitos
Python 3.6 o superior.
Bibliotecas de Python: Las bibliotecas necesarias son:
SQLAlchemy: Para gestionar la base de datos.
Pandas: Para mostrar las tareas en formato tabular.
Tkinter: Para crear la interfaz gráfica de la aplicación.
Instalación
1. Clonar el repositorio
Clona este repositorio en tu máquina local.

git clone https://github.com/tu-usuario/task-manager-app.git
cd task-manager-app
2. Crear un entorno virtual (opcional pero recomendado)
Es recomendable crear un entorno virtual para gestionar las dependencias de manera aislada.

En Windows:

python -m venv venv
venv\Scripts\activate
En macOS/Linux:

python3 -m venv venv
source venv/bin/activate
3. Instalar las dependencias
Instala las bibliotecas necesarias utilizando el archivo requirements.txt.

pip install -r requirements.txt
Si no tienes un archivo requirements.txt, puedes instalar las dependencias manualmente:

pip install sqlalchemy pandas tk
4. Crear la base de datos
La base de datos SQLite se crea automáticamente la primera vez que ejecutas la aplicación. Asegúrate de que la carpeta data/ exista en el directorio de tu proyecto.

5. Ejecutar la aplicación
Una vez que hayas instalado todas las dependencias, ejecuta el siguiente comando:

python app/task_manager_app.py
Esto abrirá la interfaz gráfica donde podrás interactuar con las tareas.

Uso
Interfaz Gráfica
Agregar Tarea: Haz clic en el botón "Agregar Tarea" para crear una nueva tarea. Se te pedirá que ingreses un título y una descripción para la tarea.
Marcar como Completada: Haz clic en "Marcar como Completada" para cambiar el estado de la tarea seleccionada a "Completada".
Eliminar Tarea: Haz clic en "Eliminar Tarea" para eliminar la tarea seleccionada de la base de datos.
Exportar Tareas: Haz clic en "Exportar Tareas" para guardar todas las tareas en un archivo JSON. Podrás elegir la ubicación y el nombre del archivo.
Importar Tareas: Haz clic en "Importar Tareas" para cargar un archivo JSON con tareas y agregar las tareas al sistema.
Mostrar Tareas
Las tareas se muestran en la interfaz en dos columnas: Descripción y Estado (Completada o Pendiente).

Exportación e Importación
Exportar: Al hacer clic en "Exportar Tareas", se crea un archivo JSON que contiene todas las tareas. Este archivo puede ser guardado y compartido.
Importar: Puedes cargar un archivo JSON que contiene tareas, y las tareas se agregarán a la base de datos.
Estructura del Proyecto
La estructura de carpetas del proyecto es la siguiente:

task-manager-app/
├── app/
│   ├── __init__.py                  # Este archivo puede estar vacío, pero debe existir
│   ├── database.py                  # Configuración de la base de datos SQLite
│   ├── task_model.py                # Definición del modelo de datos
│   ├── task_manager_app.py          # Lógica principal de la aplicación
├── data/
│   └── tasks.db                     # Base de datos SQLite donde se guardan las tareas
├── export/                          # Carpeta donde se guardan los archivos exportados
├── config.ini                       # Archivo de configuración de la aplicación
├── requirements.txt                 # Dependencias necesarias para el proyecto
└── README.md                        # Este archivo
Configuración
El archivo config.ini contiene configuraciones de red, como la dirección IP de la base de datos, que se pueden personalizar si es necesario.

[network]
ipAddress = 127.0.0.1
Contribuciones
Si deseas contribuir al proyecto, puedes hacerlo de la siguiente manera:

Fork este repositorio.
Crea una nueva rama (git checkout -b feature/nueva-funcionalidad).
Haz tus cambios y confirma tus modificaciones (git commit -am 'Añadir nueva funcionalidad').
Haz push a tu rama (git push origin feature/nueva-funcionalidad).
Abre un pull request en este repositorio.
Licencia
Este proyecto está bajo la Licencia MIT. Para más detalles, consulta el archivo LICENSE en el repositorio.
