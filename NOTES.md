Notes	

ObejctId (_id) : 12byte hex string
                 Date (4bytes) | MAC Address (3bytes) | PID (2 bytes) | Counter(3 bytes)

Whenever a find() query is done , a cursor is returned as a consequence of that                 

Equality Matches on Arrays: On the entire array
                            Based on any element
                            Based on specific element
                            More complex Matches using Operators

Examples =>

db.collName.find({"actors" : "HeroName"});   // HereIn we are querying for HeroName in the array actors , so o/p would be a any Object 			 that has an array in which this name ("HeroName") is Present
db.collName.find({"actors.0" : "HeroName"}); 
db.collName.find({"actors" : ["HeroName1" , "HeroName2"]});  //Now the order and count of these values matter in the query result

Projections in MongoDB
Reduce Network OverHead and Processing
db.collName.find({"actors":"HeroName"} , {title : 1 , _id : 0}).pretty();  // _id always is always returned but it can explicitly changed to not show