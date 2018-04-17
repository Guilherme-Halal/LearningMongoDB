# week 1:

## Star M001: MongoDB Basics

### Chapter_1_Introduction

* MongoDB Compass is the GUI tool to manager DB
* Documents are stored in collections
* A database mau contain one or more collections
* Each database and collections combinations define a namespace
* We refer to an element on Database: databaseName.collectionName.documentName

* At 'Schema' view in compas we can identfy the Value type of the elements on the Documents
* Types: strings, int32, doubles, Array, Documents, Objets, dates, 
* Can also filter the display documents
* MongoDB Documents could have Fields with Documents as Values
* Or Arrays
* And even Geospatial Data

* At Schema view we can filter collections usin JSON syntax
* Could even filter by geospatial (with a sphere centered on a dot in a map)

* Chapter 1 finished today 2018/04/06 

### Chapter 2: The MongoDB Query Language + Atlas

* CRUD - Create, Read, Update and Delete
* MogoShell (text base client):
* installation instructions [here](https://docs.mongodb.com/manual/tutorial/install-mongodb-enterprise-on-ubuntu/?_ga=2.44842404.1271538674.1523420575-1907741026.1522904146#install-mongodb-enterprise)
* Create an [Atlas Sandbox Cluster](https://cloud.mongodb.com/links/registerForAtlas)
* Chose one of the available free server in order to create a test base sandbox
* Create a userAdmin in security tab (or during the cluster creation configuration
* Security tab->IP Whitelist->ADD IP ADDRESS->ALLOW ACCESS FROM ANYWHERE->CONFIRM
* Do not generally open Atlas cluster to allow access from anywhere. (used only for learning propose)

* Conecting to the cluster that we just create:
* Using the comand on the Mongo Shell: mongo "mongodb+srv://m001-sandbox-wln8p.mongodb.net/test" --username m001-student --password *******
* Than we shoud see some validations sequences finishing on:
* MongoDB Enterprise m001-sandbox-shard-0:PRIMARY>

* Loading Data into Your Sandbox Cluster:
* The MongoSheel is a .js interpreter, so we can use it in order to executes a js scrip. Scripts that could add or retrieve some infos to the DB
* We cant also use the MongoDB queryLanguage to manipulate the DB. We will se this in the future...

* Connecting to Your Sandbox Cluster from Compass:
* On the mongoDB Atlas, in the cluster view->click in the cluster name -> identify the primary ->copy the hostname ->
* paste in the hostname box on the compass
* set to username/password
* Create a favorite name and click the 'connect' button
* now we can use all the functionalitys of the compass

* Creating Documents: insertOne():
* On the DB level we can create a new collection, it is created with 0 documents.
* We can create a new document by clicking on 'INSERT DOCUMENT' button, 
* In the MDShell we can use insertOne() method, whitch the sintax is DBName.collectionName.insertOne({elemen1: "value", element2:"value"...})

* Creating Documents: insertMany():
* this method insert a bunch os objects on the data base, as an array
* Using an second parameter on the call of the function we can insert an no-ordered lsit of objects

* Reading Documents: Scalar Fields: 

 

