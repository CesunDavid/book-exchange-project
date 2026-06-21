# Historias de Usuario - Book Exchange

## HU-01
Como usuario,
quiero registrarme en la plataforma,
para poder intercambiar libros y material.

### Criterios de aceptación (Gherkin)

Escenario: Registro exitoso

Dado que el usuario se encuentra en la pantalla de registro
Cuando ingresa un nombre, correo y contraseña válidos
Y presiona el botón "Registrarse"
Entonces el sistema crea la cuenta
Y muestra un mensaje de registro exitoso

Escenario: Registro con datos incompletos

Dado que el usuario se encuentra en la pantalla de registro
Cuando deja uno o más campos vacíos
Y presiona el botón "Registrarse"
Entonces el sistema muestra un mensaje de error
Y no crea la cuenta

## HU-02
Como usuario,
quiero publicar libros disponibles,
para que otras personas puedan encontrarlos.

### Criterios de aceptación (Gherkin)

Escenario: Publicación exitosa

Dado que el usuario ha iniciado sesión
Cuando completa la información del libro
Y presiona "Publicar"
Entonces el sistema guarda la publicación
Y muestra el libro en el catálogo

Escenario: Publicación incompleta

Dado que el usuario ha iniciado sesión
Cuando omite información obligatoria
Y presiona "Publicar"
Entonces el sistema muestra un mensaje de error
Y no registra la publicación

## HU-03
Como usuario,
quiero buscar libros por nombre o categoría,
para encontrar material fácilmente.

### Criterios de aceptación (Gherkin)

Escenario: Búsqueda exitosa

Dado que existen libros publicados
Cuando el usuario ingresa un nombre o categoría
Y realiza la búsqueda
Entonces el sistema muestra los resultados coincidentes

Escenario: Sin resultados

Dado que existen libros publicados
Cuando el usuario realiza una búsqueda sin coincidencias
Entonces el sistema muestra el mensaje
"No se encontraron resultados"

## HU-04
Como usuario,
quiero contactar a otros usuarios,
para acordar un intercambio.

### Criterios de aceptación (Gherkin)

Escenario: Contacto exitoso

Dado que el usuario visualiza un libro publicado
Cuando presiona el botón "Contactar"
Y envía un mensaje
Entonces el sistema registra el mensaje
Y notifica al propietario del libro

Escenario: Mensaje vacío

Dado que el usuario visualiza un libro publicado
Cuando intenta enviar un mensaje vacío
Entonces el sistema muestra un mensaje de error
Y no envía el mensaje
