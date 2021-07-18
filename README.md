1. Crea la estructura   del BD en sqlite en flutter añadiendo una tabla y sus respetivas columna
 “CREATE TABLE Libreria ("
"id integer primary key,"
"name TEXT,"
    "auto TEXT,"
    "catego TEXT,"
    "fecha TEXT,"
    "estado TEXT"


")"

Y especiar que el ID se auto incrementable.

Crear un login para cada una de los campo a llenar o a solicitar (“nombre , autor , categoría , fecha y estado ”) a excepción del id ya que es automático 

Al completar el formulario y hacer su validación y al presionar el botón de guardaran, todos los datos se almacenarán en la bd  en sus respectivos campos.

Automáticamente nos llevara al menú donde para poder visualizar los datos hay que refrescar la página ya sea con control + S o  en Android studio darrle en flutter hot Restar y automáticamente se mostraran los datos separados y estando en una card , posterior mente en la misma ventana tendemos varias opciones, una en un botón donde podremos añadir nuevos datos “Libros” , así como eliminar todos  los datos registrados , o si se desea eliminar un dato en específico solo basta con deslizar a la izquierda  eso usando Dismissible y aplicarle el onDismissed: (diretion) {
 DBBook.db.deleteClientWithId(item.id);}, que eliminara un solo campo  , o si se prefiere editar solo basta en darle clic a la card para poderlo editarlos campos que se quieran modificar 
