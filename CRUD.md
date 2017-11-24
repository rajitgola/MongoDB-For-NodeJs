MongoDB CRUD Operations

Some Basic Commands:

1. INSERTION

(a). db.<collectionName>.insertOne(<object>);
Example=> db.moviesScratch.insertOne({"title":"One" , "year" : "1990" , "imdb" : "Present" });;

(b). db.<collectionName>.insertMany([<object1> , <object2> ,  <objectn> ]);


2. Operators

(a). Comparison Operators
     $eq , $gt , $gte , $lt , $lte , $in , $ne , $nin

(b). Element Operators
     $exists , $type

(c). Logical Operators
     $and , $not , $or , $nor

(d). Evaluation Operators
     $regex , $mod , $text , $where

(e). Array Operators
     $all , $elemMatch , $size
