# MongoDB の基本 (日本語)

use "name_database" >> データベースを作成する

show dbs >> すべてのデータベースを表示

db >> 使用されているデータベースを表示します。

db."name_collection".insert({*json_value*}) >> コレクションを作成します。

db.dropDatabase() >> コレクションを削除する

db.createCollections("name_collection") >>  コレクションを作成します。

show collections >> shows the collections that are in the database.

db."collection_name".drop() >> コレクションを削除する

db."collection_name".find() >> コレクション内のすべてのもの (すべてのデータ) を表示します。

db.products.find({"insert document value"}) >> 検索された属性を持つ要素を探します。

db.products.find({"insert document value"}).sort({name: 1}) >> 検索された属性を持つ要素が検索され、アルファベット順に並べられます。


db.products.find().limit(3) >> すべてのアイテムを抽出するのではなく、アイテムを検索して 3 つのアイテムに制限します。
db.products.count() >> コレクション内のドキュメントの数をカウントします

db.products.find().forEach(products => print(products.name)) >> ドキュメントの名前のみを検索する ForEach を実行します

db.products.update({"name":"keyboard"}, {"price": 999.999}) >> 値、名前、およびキーボード データを持つ要素を検索し、そのドキュメント内で新しいデータを変更 (または配置) します。

db.createUser(
   {
     user: "angel",
     pwd: passwordPrompt("qwerty*"), 
     roles: [ "readWrite", "dbAdmin" ]
   }
)   << ユーザーを作成する



## これらは MongoDB の非常に基本的な概念であることに注意してください。結局のところ、これは MongoSH のショートカットとコマンドを提供するために常に更新され続けるガイドです。 :D
