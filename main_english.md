# MongoDB Basics (in English)

use "name_database" >> create a database

show dbs >> show all db's

db >> show the db that is being used.

db."name_collection".insert({*json_value*}) >> Create a collection.

db.dropDatabase() >> Delete a Collection

db.createCollections("name_collection") >>  Create a collection.

show collections >> shows the collections that are in the database.

db."collection_name".drop() >> Delete a Collection

db."collection_name".find() >> shows everything that is in a collection (all the data.)

db.products.find({"insert document value"}) >> Look for that element that has those searched attributes.

db.products.find({"insert document value"}).sort({name: 1}) >> It looks for that element that has those searched attributes and will also order it alphabetically.


db.products.find().limit(3) >> Searches for items and limits them to 3 items, instead of pulling out all items.

db.products.count() >> It will count how many documents are in the collection

db.products.find().forEach(products => print(products.name)) >> does a ForEach searching ONLY the name of the document

db.products.update({"name":"keyboard"}, {"price": 999.999}) >> It will look for an element that has a value and a name and keyboard data and in that document it will change (or place) a new data

db.createUser(
   {
     user: "angel",
     pwd: passwordPrompt("qwerty*"),  // Or  "<cleartext password>"
     roles: [ "readWrite", "dbAdmin" ]
   }
)   << Create a User



## Remember that these are very basic concepts of MongoDB, in the end this is a guide that will continue to be constantly updated, to bring MongoSH shortcuts and commands
