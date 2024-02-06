# Sistema de Gestión de Biblioteca

Este proyecto consiste en la creación de un sistema de gestión de biblioteca que permite administrar libros, revistas y usuarios de la biblioteca. El sistema permite realizar préstamos y devoluciones de libros y revistas, y llevar un registro de estadísticas de préstamos.

## Entidades

### Libros
- Propiedades: Título, Autor/Editor, Año de Publicación
- Operaciones: Creación, Listado, Edición y Eliminación

### Revistas
- Propiedades: Título, Autor/Editor, Año de Publicación
- Operaciones: Creación, Listado, Edición y Eliminación

### Usuarios de la Biblioteca
- Propiedades: Nombre, Dirección, Número de Teléfono
- Operaciones: Creación, Listado, Edición y Eliminación

### Préstamos
- Propiedades: Usuario, Artículo prestado, Fecha de inicio, Fecha de devolución estimada
- Operaciones: Creación, Listado, Devolución

## Administración de la Biblioteca

### Creación y Gestión de Usuarios
- Creación, Listado, Edición y Eliminación de usuarios.

### Creación y Gestión de Libros
- Creación, Listado, Edición y Eliminación de libros.

### Creación y Gestión de Revistas
- Creación, Listado, Edición y Eliminación de revistas.

Cada entidad tiene un identificador único para mantener la integridad referencial.

## Gestión de Préstamos y Devoluciones

### Validaciones
- No se puede prestar un artículo si otro usuario lo tiene en préstamo.
- No se puede prestar un artículo si el usuario no está registrado.
- No se puede prestar un artículo si el usuario está penalizado.

### Detalles del Préstamo
- Se registra el día de inicio del préstamo y la fecha de devolución estimada (una semana después del préstamo).
- Se aplica una escala de penalización en caso de retraso en la devolución.

## Estadísticas

### Registro de Préstamos
- Se lleva registro de todos los préstamos en un archivo.
- Cada registro incluye la fecha del préstamo, el título del artículo y el nombre del usuario.

Este sistema proporciona una gestión eficiente de la biblioteca y un seguimiento detallado de los préstamos realizados, asegurando una experiencia óptima para usuarios y administradores.
