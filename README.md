📚 Plataforma de Cursos con Django + Docker

Este proyecto es una plataforma educativa construida con Django y Docker, que permite a los usuarios autenticarse mediante OAuth2, visualizar cursos, inscribirse y activar su cuenta mediante correo electrónico. Incluye las funcionalidades requeridas en la entrega final:

Autenticación OAuth2 con Google

Vista detallada de cada curso

Listado de cursos inscritos por usuario

Envío de correo y activación de cuenta

Contenedorización completa con Docker y Docker Compose

🚀 Características principales
🔐 Autenticación OAuth2 (Google)

El sistema permite iniciar sesión mediante Google OAuth2. Incluye redirecciones, permisos, obtención de token y creación o vinculación de cuentas dentro del sistema.

📘 Ficha detallada de curso

Cada curso cuenta con una vista con la información completa: título, descripción, instructor, duración, lecciones y otros datos relevantes.

🎓 Listado de cursos inscritos

Tras iniciar sesión, el usuario puede acceder a una sección donde se muestran únicamente los cursos en los que está inscrito.

✉️ Envío de correo y activación de cuenta

El flujo de registro incluye envío de correo de bienvenida o activación y un enlace único para validar la cuenta del usuario antes de permitir el acceso.

🛠️ Tecnologías utilizadas

Django

Docker y Docker Compose

OAuth2 (Google)

SMTP (para envío de correos)

SQLite o PostgreSQL (según configuración)

🧱 Estructura del proyecto
django_docker/
│── app/
│── Dockerfile
│── docker-compose.yml
│── requirements.txt
│── manage.py
└── README.md

▶️ Cómo ejecutar el proyecto
1. Clonar el repositorio
git clone https://github.com/Maria-Paula-PR/django_docker.git
cd django_docker

2. Crear archivo .env con variables como:
GOOGLE_CLIENT_ID=xxx
GOOGLE_CLIENT_SECRET=yyy
EMAIL_HOST_USER=tu_correo
EMAIL_HOST_PASSWORD=tu_password_app

3. Construir y levantar contenedores
docker-compose up --build

4. Acceder a la aplicación
http://localhost:8000
