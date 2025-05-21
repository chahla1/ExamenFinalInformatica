# ExamenFinalInformatica

En el html, la pagina incluye un header, una seccion para mostrar las paginas del blog, un formulario para agregar 
nuevas entradas y un footer.


He usado Grid para el css ya que, como pide en las instrucciones, se pide un blog que tenga un diseño moderno y
responsivo. Grid hace que la pagina se vea bien tanto en moviles como en ordenadores, gracias a que permite
definir cuantas columnas mostrar en funcion del tamaño de pantalla. Por lo tanto, estoy utilizando Grid para que 
sea un diseño sencillo pero responsivo.

En la parte de JavaScript, he usado js para que los usuarios puedan añadir entradas sin tener que recargar la pagina. 
Ademas de esto, he añadido un boton de eliminar debajo de cada entrada para que sea mas facil borrarlo si el usuario lo desea.
Esto se consigue utilizando addEventListener para manejar eventos. Ademas de eso, uso fetchpara enviar  la entrada al backend y tambien 
para eliminar una entrada del servidor

He creado en la parte de node.js y apis un servidor con express que gestiona dos endpoints: GET /entries (devuelve todas las entradas desde un archivo entries.json) POST /entries (recibe nuevas entradas y las guarda) y  DELETE /entries/:id (elimina una entrada específica por su ID).

Podría mejorar la seguridad aplicando sanitización de entradas para evitar ataques XSS y podría usar una base de datos como SQLite o MongoDB en lugar de un archivo JSON.




