# proyecto6
---------------ANIMES: 

GET /animes: Obtiene todos los animes.

Respuesta: Lista de objetos de animes.
GET /animes/
: Obtiene un anime por su ID.

Parámetro: id (string) - ID del anime.
Respuesta: Objeto del anime correspondiente.
GET /animes/categoria/
: Obtiene animes por estilo o categoría.

Parámetro: categoria (string) - Estilo o categoría del anime.
Respuesta: Lista de animes que coinciden con el estilo.
GET /animes/precio/
: Obtiene animes con un precio menor o igual al especificado.

Parámetro: precio (number) - Precio máximo.
Respuesta: Lista de animes que cumplen con el filtro de precio.
POST /animes: Crea un nuevo anime.

Cuerpo: Objeto JSON con los datos del anime.
Respuesta: Objeto del anime creado.
PUT /animes/
: Actualiza un anime existente.

Parámetro: id (string) - ID del anime a actualizar.
Cuerpo: Objeto JSON con los datos actualizados.
Respuesta: Objeto del anime actualizado.
DELETE /animes/
: Elimina un anime por su ID.

Parámetro: id (string) - ID del anime a eliminar.
Respuesta: Objeto del anime eliminado.

--------------------CREADORES: 

GET /creadores: Obtiene todos los creadores.

Respuesta: Lista de objetos de creadores.
GET /creadores/
: Obtiene un creador por su ID.

Parámetro: id (string) - ID del creador.
Respuesta: Objeto del creador correspondiente.
POST /creadores: Crea un nuevo creador.

Cuerpo: Objeto JSON con los datos del creador.
Respuesta: Objeto del creador creado.
PUT /creadores/
: Actualiza un creador, añadiendo nuevos animes a su lista sin duplicados.

Parámetro: id (string) - ID del creador a actualizar.
Cuerpo: Objeto JSON con los nuevos animes a agregar.
Respuesta: Objeto del creador actualizado.
DELETE /creadores/
: Elimina un creador por su ID.

Parámetro: id (string) - ID del creador a eliminar.
Respuesta: Objeto del creador eliminado.


DEPENDENCIAS: 
Express: Framework para aplicaciones web.
Mongoose: ODM para MongoDB.
dotenv: Manejo de variables de entorno.
Nodemon: Recarga automática para desarrollo.
