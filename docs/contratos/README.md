Arquitectura API - Book Exchange

Registro de Usuario
Endpoint:

POST /usuarios

Motivo: Se envían datos para crear un nuevo usuario.

JSON:

{ "nombre": "Juan Perez", "correo": "juan@gmail.com", "contrasena": "12345678" }

Publicar Libro
Endpoint:

POST /libros

Motivo: Se envían datos para registrar un libro disponible.

JSON:

{ "titulo": "Python para Principiantes", "autor": "Carlos Ruiz", "categoria": "Programacion", "descripcion": "Libro en buen estado", "estado": "Disponible" }

Buscar Libros
Endpoint:

GET /libros

Motivo: Obtiene la lista de libros publicados.
