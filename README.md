# Cinema
Aplicación web para la administración general de un cine.
Proyecto completo aplicando tecnologias web (front-end + back-end). HTML, CSS, Javascript, PHP y MySQL.

## Requerimientos funcionales
### Parte de administración
En esta sección se permitirá la gestión de distintos aspectos del cine (siempre previa autenticación). Comprende tareas de administración como gestionar las películas, horarios y salas.

#### **Gestión de Películas**
  1. Crear una nueva película.
  2. Eliminar una película existente.
  3. Modificar una película existente.
  4. Consultar una película existente.
  5. Buscar y listar películas según diferentes criterios (género, año, nacionalidad, etc.).
  6. Para cada película se gestionará la siguiente información:
     - Identificador del película: este identificador debe ser un valor entero autoincremental.
     - Nombre.
     - Duración.
     - Año.
     - Nacionalidad.
     - Director.
     - Actores principales.
     - Actores Secundarios.
     - Nombre de su sitio Web oficial.
     - Sinopsis.
     - Imagen referencial.
     - Genero de película: este campo deberá estar asociado a una categoría existente.
     - Comentarios.

#### **Gestión de Salas**
  1. Crear una nueva sala.
  2. Habilitar/Deshabilitar una sala.
  3. Consultar disponibilidad de sala.
  4. Para cada sala se gestionará la siguiente información:
     - Identificador de sala: este identificador debe ser un valor entero autoincremental.
     - Capacidad de asientos.
     - Disponibilidad (habilitada /deshabilitada).


#### **Gestión de cartelera de la semana actual**
La aplicación deberá mostrar y actualizar la cartelera vigente del cine. La cartelera incluye todas las películas que se están proyectando, así como la asignación de sala y horarios, para cada película se debe incluir una imagen correspondiente.

#### **Gestionar la cuenta de acceso al sistema**
La aplicación destinada a varios usuarios administradores, por lo que se gestionará cuentas con todos los privilegios posibles y permitirá editar la siguiente información de la cuenta:
- Apellido de la persona que administra la cuenta.
- Nombres de la persona que administra la cuenta.
- Nombre de usuario: identificador que permitirá acceder a la cuenta.
- Contraseña: clave que permitirá acceder a la cuenta.
- Correo electrónico: correo personal del administrador de la cuenta, el cual será necesario para poder recuperar la contraseña.
- Tiempo de notificación: intervalo de tiempo previo a la ocurrencia de cualquier evento en un recordatorio. La Agenda Web tendrá en cuenta este tiempo para notificar previamente la proximidad de un evento.

#### **Recuperación de la clave de la cuenta de acceso**
La aplicación deberá permitir al usuario poder recuperar sus datos. El usuario podrá hacer uso de esta funcionalidad desde la página de login o autenticación de la aplicación Web. Los datos que el usuario recibirá en su correo electrónico serán:
- El nombre de usuario de la cuenta.
- Una contraseña generada aleatoriamente, con una longitud mínima de 6 caracteres. Esto implica que la misma será reseteada en la base de datos y enviada al usuario.

### Parte usuario general
Comprende funcionalidades de la parte de usuario, como puedan ser consultas de cartelera actual del cine, compra de entradas, registrar opinión sobre las películas (esta última funcionalidad requiere identificarse en el sistema).

#### **Registro de un nuevo usuario general**
La aplicación deberá permitir a un usuario nuevo poder registrarse ingresando la siguiente información:
- Apellido de la persona
- Nombres de la persona
- Nombre de usuario. Identificador que permitirá acceder a la cuenta.
- Contraseña. Clave que permitirá acceder a la cuenta.
- Correo electrónico.

#### **Recuperación de la clave de la cuenta de acceso**
La aplicación deberá permitir al usuario poder recuperar sus datos. El usuario podrá hacer uso de esta funcionalidad desde la página de login o autenticación de la aplicación Web. Los datos que el usuario recibirá en su correo electrónico serán:
- El nombre de usuario de la cuenta.
- Y una contraseña generada aleatoriamente, con una longitud mínima de 6 caracteres. Esto implica que la misma será reseteada en la base de datos y enviada al usuario.

#### **Compra de entradas para ver una película**
La aplicación deberá emitir una/s entrada/s una vez seleccionada la película, día, hora, sala y asientos a comprar, se pedirá un número de tarjeta al que cargar el importe. Si la compra se ha ejecutado con éxito se proporcionará un número de referencia de la compra.

#### **Introducción de Comentario para una película**
La aplicación permitirá a un usuario general conectado poder registrar la opinión sobre una película determinada.

#### **Búsqueda de una película**
La aplicación permitirá a un usuario general buscar y listar películas según diferentes criterios (género, año, nacionalidad, etc.).

#### **Visualización de la cartelera vigente de la semana en curso**
La aplicación deberá listar en su pagina de inicio las películas actualmente en proyeción y, opcionalmente, aquellas próximas a estrenarse.

## Requerimientos no funcionales
  1. La contraseña de acceso del usuario deberá mantenerse encriptada en la base de datos, mediante algún algoritmo de encriptación conocido, por ejemplo con alguna variante de md5 o sha.
  2. Cualquier listado que emita la aplicación Web, deberá tener la opción de exportarlo a un documento PDF.
  3. Al consultar la información de una película, se deberá poder exportar la misma a un documento PDF.
  4. La aplicación Web deberá presentar una interfaz amigable, teniendo en cuenta lo siguiente:
     - El menú principal de la aplicación deberá ser accesible desde cualquier página.
     - Se podrá finalizar la sesión actual desde cualquier página de la aplicación.
     - Cualquier operación de edición o borrado de datos deberá solicitar una confirmación al usuario.
     - Los reportes PDF deberán mostrarse en una nueva ventana del navegador.
     - La introducción de datos del tipo fecha, deberán hacerse mediante un calendario.
