# Pasos iniciales - FullSatck (Contenido para BackEnd)

## Descripción de conocimientos adquiridos

Con los conocimientos adquiridos en la parte del BackEnd ahora ya podrás hacer uso de las siguientes herramientas/tecnologías para construir una aplicación robusta y completamente funcional:

- Persistencia de información con el uso de bases de datos, podrás utilizar el manejador de base de datos que sea de tu agrado, así como también elegir entre un sistema **SQL** o **NoSQL** dependiendo tus necesidades. Estas pueden incluir **MySQL, PostgreSQL, MongoDB, H2**, etc.
- Crear una **API tipo REST** la cuál servida como una capa de comunicación entre el FrontEnd y el BackEnd, con esta arquitectura serás capas de delegar las funcionalidades sobre procesamiento/validación de información al BackEnd, con operaciones tipo CRUD (_Create, Read, Update, Delete_, lo que en español denominamos como **_Crear, Leer, Actualizar y Eliminar_** información de una Base de Datos.
- Así mismo, crearás documentación que será de gran ayuda para los equipos de **FrontEnd** y **BackEnd** en el cual se definirán de manera muy clara las operaciones que tu **API REST** realizará, en este caso utilizaremos un tipo de formato llamado Swagger, del cuál tendrás disponible un módulo completo con la explicación y herramientas necesarias para que puedas realizarlo sin ningún inconveniente.
- Darás seguimiento a tu proyecto utilizando la herramienta **git**, esta te ayudará a llevar el control de cambios del mismo, pudiendo hacer un rollback de tu aplicación a un estado anterior, y mejor aún podrás, en caso de que así lo desees, compartir el repositorio para que más personas puedan aportar ideas nuevas o quizás ayudarte con la corrección de posibles errores o bugs en el mismo.
- En este curso de **BackEnd** también te daré las herramientas necesarias en caso de que quieras publicar tu API en internet, haciendo uso de tecnologías en la nube como **AWS de Amazon**, con el cuál podrás fácilmente publicar tu **API** y que esté al alcance de cualquiera que desee interactuar con ella.
- En caso de ser necesario, también podrás hacer uso de contenedores **Docker** para el uso de, por ejemplo, manejadores de base de datos.

## Descripción del proyecto final

Descripción general:

- Se realizará una aplicación la cuál permitirá interactuar con un **_catálogo de productos_** con las siguientes operaciones:
    + Crear productos
    + Actualizar productos
    + Leer productos
    + Eliminar productos
- Se deberá contemplar también la funcionalidad para **_registrar y autenticar usuarios_**, los cuales serán los únicos con privilegios para poder interactuar con el catálogo de productos.
- Dado que esta aplicación se tiene pensada para ser expuesta como una **API REST**, se debe tener en mente que toda la información de entrada y salida deberá estar en un formato **JSON** para que pueda ser utilizada en conjunto con **Swagger**

### Requerimientos técnicos:

- **JDK** version 8 o superior
- Uso del framework **SpringBoot** para poder ejecutar una aplicación de tipo Microservicio
- Uso de **Gradle** o **Maven** para el ciclo de vida de tu proyecto, el cuál deberá incluir pruebas unitarias de toda tu funcionalidad.
- Diferentes _endpoints_ para realizar las funcionalidades referentes a productos y Usuarios.
- En cuanto a Base de datos, se podrá utilizar cualquier manejador (**_MySQL, PostgreSQL, MongoDB, H2_**, etc.), contemplando las siguientes tablas:

__Tabla:__ _Productos_

|    Campo    |  Tipo   |       Descripción        |
|:-----------:|:-------:|:------------------------:|
| idProducto  |   int   |      llave primaria      |
|   nombre    | varchar |     Nombre producto      |
| descripción | varchar | Descripción del producto |
|   origen    | varchar |   Origen del producto    |

__Tabla:__ _Usuarios_

|   Campo   |  Tipo   |       Descripción        |
|:---------:|:-------:|:------------------------:|
| idUsuario |   int   |      llave primaria      |
|  nombre   | varchar |     Nombre producto      |
|  correo   | varchar |    Correo electrónico    |
| password  | varchar | Password cifrado con md5 |

_** Revisar con FrontEnd si considera necesario agregar mas campos. La estructura de las tablas es sugerida._

## Entregable

Tu entregable será la dirección de tu repositorio **git**, el cual deberá contener lo siguiente:

- Archivo **README.md** con una explicación sobre tu proyecto, herramientas utilizadas (_Version de JDK, Gradle, Maven, Spring, etc._)
- En caso de aplicar, las _instrucciones detalladas para ejecutar_ el proyecto en un entorno local.
- _Posibles mejoras_ que consideres relevantes en tu aplicación.
