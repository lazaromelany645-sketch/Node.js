
# APLICACIONES NODEJS - EXPRESS

## DESCRIPCIÓN

Aplicación web desarrollada con **Node.js y Express** que permite gestionar los datos de un sistema de **logística y activos** mediante una API REST y una interfaz web en HTML.

El sistema permite realizar operaciones CRUD sobre los activos y gestionar sus categorías.

## REQUERIMIENTOS

Para ejecutar el proyecto se necesita:

* **Node.js**
* **Express**
* **MySQL**
* **MySQL2**
* **Knex.js**
* **HTML**
* **CSS**
* **JavaScript**

## FUNCIONES

El sistema permite:

* Registrar activos.
* Mostrar activos.
* Editar activos.
* Eliminar activos.
* Registrar categorías.
* Consultar categorías.
* Conectar el frontend HTML con la API.

# INSTALACIÓN

## 1. Descargar o clonar el proyecto

Descargar el proyecto y abrir la carpeta en Visual Studio Code.

## 2. Instalar las dependencias

Ejecutar en la terminal:

bash
npm install

## 3. Crear la base de datos

En MySQL crear la base de datos:

sql
CREATE DATABASE logistica;


## 4. Ejecutar las migraciones

Ejecutar:

bash
npm run migrate


## 5. Insertar los datos iniciales

Ejecutar:

bash
npm run seed


## 6. Iniciar el servidor

Ejecutar:
bash
npm start


El servidor estará disponible en:

http://localhost:3000


# ACCESO AL SISTEMA

## Página principal

http://localhost:3000


## Lista de activos


http://localhost:3000/activos/listar.html

## Registrar activo

text
http://localhost:3000/activos/registrar.html

# API REST

## ACTIVOS

| Método | Ruta               | Función          |
| ------ | ------------------ | ---------------- |
| GET    | `/api/activos`     | Mostrar activos  |
| POST   | `/api/activos`     | Registrar activo |
| PUT    | `/api/activos/:id` | Editar activo    |
| DELETE | `/api/activos/:id` | Eliminar activo  |

## CATEGORÍAS

| Método | Ruta                  | Función             |
| ------ | --------------------- | ------------------- |
| GET    | `/api/categorias`     | Mostrar categorías  |
| POST   | `/api/categorias`     | Registrar categoría |
| PUT    | `/api/categorias/:id` | Editar categoría    |
| DELETE | `/api/categorias/:id` | Eliminar categoría  |

# BASE DE DATOS

El proyecto utiliza la base de datos:

text
logistica

## Tablas principales

* `categorias`
* `activos`

La tabla `activos` está relacionada con la tabla `categorias`.

# CRUD

## CREATE

Permite registrar nuevos activos.

## READ

Permite consultar y mostrar los activos registrados.

## UPDATE

Permite modificar la información de los activos.

## DELETE

Permite eliminar activos registrados.

# IMPORTANTE

Los archivos HTML deben abrirse utilizando el servidor de **Node.js y Express**.

Por ejemplo:

text
http://localhost:3000/activos/listar.html


**No se debe abrir directamente el archivo HTML con:**

text
file:///


Esto puede provocar el error:

text
TypeError: Failed to fetch


porque el navegador no estará realizando las peticiones a la API desde el servidor de Express.

# MIGRACIONES Y SEMILLAS

Las migraciones se utilizan para crear las tablas de la base de datos:

bash
npm run migrate


Las semillas permiten insertar datos iniciales:

bash
npm run seed


# TECNOLOGÍAS UTILIZADAS

**Node.js**
Entorno utilizado para ejecutar JavaScript en el servidor.

**Express**
Framework utilizado para crear la API REST.

**MySQL**
Sistema gestor de base de datos.

**Knex.js**
Herramienta utilizada para las migraciones y consultas a la base de datos.

**HTML, CSS y JavaScript**
Tecnologías utilizadas para la interfaz del sistema.


