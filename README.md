# Prueba técnica para el puesto de programador jr FullStack - Fantasticfy

La siguiente prueba técnica tiene como propósito evaluar los conocimientos del desarrollador en el stack tecnológico que se utiliza en Fantasticfy. El desarrollador debe tener en cuenta las siguientes consideraciones:

- Deberá hacer uso de las tecnologías indicadas
- Podrá hacer uso de su criterio para implementar las soluciones siempre y cuando el resultado final sea el esperado
- Los estilos de la aplicación web deberán manejarse con CSS puro, sin hacer uso de librerías de estilos.

## Requerimiento general

Se necesita extender la funcionalidad del desarrollo previamente realizado. Dentro de la aplicación web debe existir una página para poder ver y editar la información de los usuarios, así como una nueva columna en la tabla de usuarios para navegar a esta página y un botón para eliminar el usuario. Se deberán crear los endpoints necesarios en el servidor API para manejar estos servicios.

## Componentes de la prueba

- Servidor API REST.
- Base de datos no relacional.
- Aplicación web.

## Servidor API REST

### Ecosistema

- **Servidor:** [Node Js](https://nodejs.org/en).
- **Base de datos:** [MongoDB](https://www.mongodb.com/) (Sugerencia: [Mongoose](https://www.npmjs.com/package/mongoose)).
- **API:** A elección del desarrollador (Sugerencia: [Express](https://www.npmjs.com/package/express)).

### Requerimiento

Agregar las siguientes rutas al servidor API:

#### **GET /users/:id**

Obtener un usuario por su id.

#### **DELETE /users/:id**

Eliminar un usuario de la base de datos.

#### **PUT /users**

Extender la funcionalidad para que permita actualizar un usuario.

## Aplicación web

### Ecosistema

- ReactJs o Vanilla JS (Sugerencia: [NextJs](https://nextjs.org/docs)).

### Requerimiento

Agregar nuevas funcionalidades y página a la aplicación:

#### Página principal

Agregar una nueva columna a la tabla de usuarios llamada acciones la cual tiene que dar la posibilidad de:

- Navegar a la página de detalle del usuario.
- Eliminar el usuario.

Además se deberán agregar nuevos componentes a la tabla:

- Agregar un buscador en la tabla para poder filtrar los usuarios por su nombre, nombre de usuario, email o dirección.
- Dar la posibilidad de ordenar los resultados por orden alfabético.

#### Página de detalle de usuario

Deberá mostrar la información completa del usuario. Debe de poderse modificar los datos del usuario y hacer uso del endpoint para actualizar usuarios del servidor API.
