MongoDB CRUD Operations

Some Basic Commands:

1. INSERTION

(a). db.<collectionName>.insertOne(<object>);
Example=> db.moviesScratch.insertOne({"title":"One" , "year" : "1990" , "imdb" : "Present" });;

(b). db.<collectionName>.insertMany([<object1> , <object2> ,  <objectn> ]);