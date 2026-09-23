# 📝 To-Do List App (Flask + MySQL)

Aplicación web simple para gestionar tareas (To-Do List), con backend en **Flask**, base de datos **MySQL** y frontend en **HTML, CSS y JavaScript**.

---

## 🧱 Requerimientos funcionales

### 🔹 Backend (Flask)
- [ ] **Configurar el entorno del proyecto**  
  - Crear entorno virtual.  
  - Instalar dependencias (`Flask`, `Flask-SQLAlchemy`, `mysqlclient` o `pymysql`, etc.).  
  - Configurar conexión a la base de datos en `config.py`.

- [ ] **Diseñar el modelo de base de datos**  
  - Crear tabla `tasks` con los campos:  
    - `id` (INT, PK, autoincremental)  
    - `title` (VARCHAR)  
    - `description` (TEXT)  
    - `is_done` (BOOLEAN)  
    - `created_at` (DATETIME)

- [ ] **Implementar rutas API REST**  
  - `GET /tasks` → obtener todas las tareas.  
  - `GET /tasks/<id>` → obtener una tarea específica.  
  - `POST /tasks` → crear una nueva tarea.  
  - `PUT /tasks/<id>` → actualizar una tarea existente.  
  - `DELETE /tasks/<id>` → eliminar una tarea.

- [ ] **Validaciones y manejo de errores**  
  - Validar datos de entrada antes de crear o modificar tareas.  
  - Manejar errores 404 (no encontrado) y 500 (error interno) con mensajes JSON claros.

- [ ] **Pruebas básicas del backend**  
  - Crear tests unitarios o de integración usando `pytest` o `unittest`.  
  - Verificar que todos los endpoints funcionen correctamente.

---

### 🔹 Frontend (Flask + HTML, CSS, JavaScript)
- [ ] **Diseño de interfaz**  
  - Crear plantillas con **Jinja2** (por ejemplo, `index.html`, `edit.html`).  
  - Página principal que muestre la lista de tareas.  
  - Formulario para agregar nuevas tareas.  
  - Botones para editar y eliminar tareas.  
  - Checkbox o toggle para marcar una tarea como completada.

- [ ] **Integración con Backend Flask**  
  - Usar rutas Flask para renderizar las vistas y manejar formularios (`@app.route`).  
  - Implementar llamadas **AJAX** con `fetch()` o `axios` para actualizar tareas sin recargar la página.  
  - Devolver datos en formato **JSON** desde el backend cuando corresponda.

- [ ] **Estilo y usabilidad**  
  - Aplicar diseño simple (Bootstrap o Tailwind).  
  - Mostrar notificaciones de éxito o error al usuario.  
  - Asegurar una experiencia fluida en escritorio y móvil.

- [ ] **Gestión de archivos estáticos**  
  - Organizar los recursos en carpetas `/static/css`, `/static/js`, `/static/img`.  
  - Configurar Flask para servir estos archivos correctamente.

---

### 🔹 Base de datos (MySQL)
- [ ] **Configuración de esquema**  
  - Crear base de datos `todo_app`.  
  - Definir usuario, contraseña y privilegios.  
  - Ejecutar script de creación de tabla.

- [ ] **Persistencia y migraciones**  
  - Usar `Flask-SQLAlchemy` o `Flask-Migrate` para mantener el esquema actualizado.

---

### 🔹 Extras / Mejora opcional
- [ ] **Autenticación de usuarios**  
  - Registro e inicio de sesión.  
  - Asociar tareas a cada usuario.

- [ ] **Despliegue**  
  - Despliegue en PythonAnywhere

---

### ✅ Objetivo final
Tener una aplicación funcional donde el usuario pueda:
- Crear, listar, editar y eliminar tareas.
- Marcar tareas como completadas.
- Guardar los datos de forma persistente en MySQL.
- Interactuar con una interfaz web sencilla y moderna.


## Cómo actualizar el checklist

Marcá cada requisito con `[x]` cuando esté completo y dejalo como `[ ]` mientras siga pendiente. Para cambios que requieren código, abrí un issue pequeño y vinculá el Pull Request que lo resuelve.
