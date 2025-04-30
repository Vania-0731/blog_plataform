# 📝 Django Blog Platform - Mastering ORM Relationships

Este proyecto es una plataforma de blog desarrollada con Django, con enfoque en dominar el uso del ORM (Object-Relational Mapping). Aprenderás a manejar relaciones entre modelos, consultas personalizadas, filtros complejos y anotaciones básicas.

## 🚀 Características Principales

- Relaciones entre modelos: One-to-Many, Many-to-Many y con usuarios.
- Vistas basadas en clases para manejar publicaciones, categorías, etiquetas y comentarios.
- Interfaz administrativa personalizada.
- Sistema de comentarios con aprobación.
- Gestión de archivos estáticos (CSS/JS).
- Plantillas responsivas y personalizadas.
- Base de datos con datos de ejemplo.
- Consultas avanzadas usando ORM.
- Extensible con módulos como perfiles de usuario y análisis.

---

## 🛠️ Instalación y Configuración

### 1. Clona el repositorio

```bash
git clone https://github.com/Vania-0731/blog_plataform.git
cd blog_plataform
```

### 2. Crea y activa un entorno virtual

```bash
python3 -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate
```

### 3. Instala dependencias

```bash
pip install -r requirements.txt
```

### 4. Aplica migraciones y crea la base de datos

```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Carga datos de ejemplo

```bash
python manage.py seed_data
```

### 6. Inicia el servidor de desarrollo

```bash
python manage.py runserver
```

---

## 🌐 Acceso

- Sitio web: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
- Admin: [http://127.0.0.1:8000/admin/](http://127.0.0.1:8000/admin/)
  - Usuario: `admin`
  - Contraseña: `admin123`

---

## 🧪 Pruebas y Consultas ORM

Puedes explorar consultas avanzadas ejecutando:

```bash
python manage.py shell
```

Ejemplos:

```python
from blog.models import Post

Post.blog_objects.published()
Post.blog_objects.by_tag('django')
```

---

## 🧩 Estructura del Proyecto

```
blog_platform/
├── src/
│   ├── blog/         # Aplicación principal
│   ├── config/       # Configuración del proyecto
│   ├── templates/    # Plantillas HTML
│   ├── static/       # Archivos CSS/JS
├── venv/             # Entorno virtual
├── requirements.txt  # Dependencias
```

---

## 🔮 Posibles Extensiones

- Sistema de perfiles de usuario
- Dashboard de analíticas
- Herramientas editoriales
- Comentarios en hilo y markdown
- Búsqueda avanzada
- Integración con redes sociales y newsletters

---
