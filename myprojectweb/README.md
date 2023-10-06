# Aplicación en Flask para manejo de Tareas #

Este es un simple proyecto de aplicación web utilizando Flask y una base de datos Access para gestionar tareas. 
Aquí hay una guía rápida sobre cómo funciona y cómo puedes usarlo.

# Estructura del Proyecto #
El proyecto consta de tres archivos principales:

1. **app.py**: Contiene el código principal de la aplicación Flask.
2. **database.accdb**: La base de datos Access que almacena las tareas.
3. **templates/tareas.html**: Una plantilla HTML para mostrar las tareas en la interfaz de usuario.

# Configuración de la Base de Datos #
La conexión a la base de datos se establece en el archivo `app.py` usando el módulo `pyodbc`.
Asegúrate de tener el controlador de Microsoft Access instalado y actualiza la ruta del archivo de base de datos según tu configuración.

# Rutas de la Aplicación #
- **'/':** Muestra todas las tareas almacenadas en la base de datos en una página web.
- **'/agregar_tarea':** Permite agregar nuevas tareas mediante un formulario HTML y redirige a la página principal.
- **'/completar_tarea/<int:tarea_Id>':** Marca una tarea como completada o no completada y redirige a la página principal.
- **'/eliminar_tarea/<int:tarea_Id>':** Elimina una tarea de la base de datos y redirige a la página principal.

# Uso #
1. Asegúrate de tener Python y Flask instalados en tu sistema.
2. Configura la base de datos y actualiza la conexión en `app.py`.
3. Ejecuta `app.py` y abre tu navegador en `http://127.0.0.1:5000/`.
4. Interactúa con la aplicación para agregar, completar o eliminar tareas.

# Dependencias #
Asegúrate de tener instaladas las dependencias necesarias ejecutando:

pip install Flask pyodbc

¡Disfruta gestionando tus tareas con esta simple aplicación web!
