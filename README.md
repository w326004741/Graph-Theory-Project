# Graph-Theory-Project
 
 This is a Neo4j database on the GMIT timetable.
 
 ## Installation
     Neo4j DownloadLink https://neo4j.com/download/
     
 
 
 
 
## Node Labels: 
        Course, Lecturer, Room, Subject, Year.
         
 
## Relationship types: 
        Lecturer, Room_For, Topic_Of, Year_Of. 
        
    

## Property Keys: 
        Day, RoomNumber, StudentGroup, Time, Type, course, gr, name, time, type, week, year.        
 ##  Usage
     Create a node with the label Person, and one property: 
     create (n:Person {name:"Jason"}) return n;
     
     
     
     Find The Node(s) with label Person and their name property :
     Match (n:Person) where n.name="Jason" return n;
     
     
     
     Create relationship:
     match (a:Person{name:"Jason"}),(b:Person{name:"Jack"}) MERGE (a)-[r:Friends{since:"1998"}]->(b);
     
     
     
     Set node property:
     match(n:Person{name:"Jack"}) set n.age=34 return n;
     match(n:Person{name:"Jack"}) remove n.age return n;
     
     
     
     Delete all nodes:
     match (n) delete n;
     
     
     
     Delete relationship:
     match (n)-[r]-(m) delete r;
     
     
     
     Delete All relationship and nodes:
     match (n) optional match (n)-[r]-() delete n,rfile:///Users/weichenwang/Desktop/Project%20Screenshot.png
     
     
     
     Find All relationship and nodes: 
     match (n) return n;

