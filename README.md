# Server
try to all of the server





develop preparation
1st. install node.js
// https://nodejs.org/ko/download/

2st. install mongodb
// download taz file, cd download file decompresion and cd this directory, tar -zxvf mongodb-macos-x86_64-4.2.1.tgz <-- file name.tgz , sudo cp ./bin/* /usr/local/bin

3st. mongodb excute
// command 'mongod --dbpath /storage address', MongoDB Shell enter command 'mongo'

4st. create project
// npm init --> product 'package.json'

5st. package install
// npm install --save express mongoose body-parser
 5-1) express: web framework
 5-2) body-parser: data process middleware
 5-3) mongoose: MongoDB interlock library
 
 
Directory architecture
- models/
----- book.js
- node_modules/
- routes
----- index.js
- app.js
- package.json


Create webServer use Express
- API list
ROUTE	METHOD	DESCRIPTION
-api/books	                GET	      all of book data read
-api/books/:book_id	        GET	       _id value to data read
-api/books/author/:author	  GET	      author value to data read 
-api/books	                POST    	book data create
-api/books/:book_id	        PUT     	book data update
-api/books/:book_id	        DELETE	  book data remove


