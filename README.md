

Proyecto CRUD para administrar activos utilizando Node.js, Express, MySQL y HTML.

Tecnologías
Node.js
Express
MySQL
Knex.js
HTML
CSS
JavaScript
Funciones

El sistema permite:

Registrar activos.
Mostrar activos.
Editar activos.
Eliminar activos.
Registrar y consultar categorías.
Instalación
Descargar o clonar el proyecto.
Instalar las dependencias:
npm install
Crear la base de datos en MySQL:
CREATE DATABASE logistica;
Ejecutar las migraciones:
npm run migrate
Insertar los datos iniciales:
npm run seed
Iniciar el servidor:
npm start
Acceso

Abrir en el navegador:

http://localhost:3000

Para ver los activos:

http://localhost:3000/activos/listar.html

Para registrar un activo:

http://localhost:3000/activos/registrar.html
API

Activos
GET    /api/activos
POST   /api/activos
PUT    /api/activos/:id
DELETE /api/activos/:id

Categorías
GET    /api/categorias
POST   /api/categorias
PUT    /api/categorias/:id
DELETE /api/categorias/:id
Base de datos

El proyecto utiliza la base de datos:

logistica

Tablas principales:

categorias
activos


El archivo HTML debe abrirse desde el servidor:

http://localhost:3000/activos/listar.html

No se debe abrir directamente con:

file:///
