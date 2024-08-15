# MongoDB Básico (en Español)

use "nombre_de_base_de_datos" >> crear una base de datos

show dbs >> mostrar todas las db's

db >> mostrar la db qué se esta usando.

db."nombre de la colección".insert({*insertar valor JSON*}) >> Crea una colección.

db.dropDatabase() >> Elimina la base de datos.

db.createCollections("nombre_de_la_colección") >> crea una colección.

show collections >> muestra las colecciones qué están en la base de datos.

db."colección insertada".drop() >> Elimina una colección

db."inserte colección".find() >> muestra todo lo qué hay en una colección (todos los datos.)

db.products.find({"inserte valor del documento"}) >> busca aquel elemento qué tenga esos atributos buscados.

db.products.find({"inserte valor del documento"}).sort({name: 1}) >> busca aquel elemento qué tenga esos atributos buscados y además lo va a ordenar alfabéticamente.


db.products.find().limit(3) >> Busca los elementos y los limita a 3 elementos, en vez de sacar todos los elementos.

db.products.count() >> va a contar cuantos documentos se encuentra en la colección

db.products.find().forEach(products => print(products.name)) >> hace un ForEach buscando SOLAMENTE el nombre del documento

db.products.update({"name":"keyboard"}, {"price": 999.999}) >> va a buscar un elemento qué tenga un valor y un dato de nombre y keyboard y en ese documento le va a cambiar (o colocar) un nuevo dato

db.createUser(
   {
     user: "angel",
     pwd: passwordPrompt("qwerty*"),  // Or  "<cleartext password>"
     roles: [ "readWrite", "dbAdmin" ]
   }
)   << crear usuario

## Está es una guia muy sencilla de comandos de MongoSH, constantemente estó se va a actualizar, espero qué les sirva :) 🚀✨✨
