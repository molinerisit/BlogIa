BlogIa - Aplicación de Gestión de Blogs

Descripción
BlogIa es una aplicación de gestión de blogs que permite a los usuarios crear, editar, y gestionar
entradas de blog, comentarios, valoraciones y categorías. Está construida utilizando React en el
frontend y Express en el backend, con una base de datos MongoDB. La aplicación también integra
servicios externos como Cloudinary para la gestión de imágenes y OpenAI para generación de
contenido.
Requisitos previos
Antes de ejecutar la aplicación, asegúrate de tener instalados los siguientes programas en tu
máquina:
- Node.js (versión 14 o superior)
- MongoDB (localmente o configurado en la nube)
Estructura del proyecto
Frontend (client): Carpeta que contiene todo el código de la interfaz de usuario, creada con React.
Backend (server): Carpeta que contiene la API construida con Express y MongoDB como base de
datos.

Configuración del entorno

Debes crear un archivo .env en la raíz de la carpeta del backend (server) con las siguientes
variables de entorno. No olvides reemplazar las credenciales con tus propios datos antes de subir el
proyecto a un repositorio público:

MONGO_URI=mongodb://localhost:27017/BlogIa
DEV_EMAIL=admin@gmail.com
DEV_PASSWORD=1234
PORT=5000
JWT_SECRET=tu_clave_secreta
ACCESS_TOKEN_SECRET=clavesecreta
CLOUDINARY_CLOUD_NAME=tu_cloud_name
CLOUDINARY_API_KEY=tu_api_key
CLOUDINARY_API_SECRET=tu_api_secret
OPENAI_API_KEY=tu_api_key_openai

Instalación
1. Clonar el repositorio:
 git clone https://github.com/usuario/blogia.git
 cd blogia

2. Instalar dependencias:

 Frontend (client):
 cd client
 npm install

 Backend (server):
 cd ../server
 npm install

Ejecutar la aplicación

1. Iniciar MongoDB
 Asegúrate de que MongoDB esté corriendo en tu sistema.

2. Iniciar el Backend
 Desde la carpeta server, ejecuta:
 node index.js

3. Iniciar el Frontend
 Desde la carpeta client, ejecuta:
 npm start
 
 Esto abrirá la aplicación en http://localhost:3000.


Características principales
Autenticación y Autorización con JWT.
Gestión de Blogs: Crear, editar y eliminar publicaciones.
Comentarios y Valoraciones.
Cargas de Imágenes con Cloudinary.
Programación de Tareas con node-cron.
Estructura de Archivos Principal
client/src/App.js: Componente principal del frontend.
client/src/pages/: Contiene las diferentes páginas.
server/index.js: Punto de entrada del backend.
server/routes/: Contiene rutas de usuarios, posts, etc.
Consideraciones
Seguridad: Mantén seguras las claves secretas de JWT, Cloudinary y OpenAI.
.env: Nunca subas tu archivo .env a un repositorio público.

Comandos útiles

Frontend:
 npm start: Inicia en modo desarrollo.
 npm run build: Compila para producción.
Backend:
 npm start: Inicia el servidor.
 npm run dev: Usa nodemon para reinicios automáticos.

Versión: 1.0.0

Créditos
Autor: Julian Molineris

