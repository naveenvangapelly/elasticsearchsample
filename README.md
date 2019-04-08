# es-java-client-sample
 Prerequisite : Java 8 and Later version 

### Start ElasticSearch
1) Download elasticsearch from [here](https://www.elastic.co/downloads/elasticsearch)   
2) Extract downloaded elasticsearch     
3) cd elasticsearch-X.X.X       
4) $ bin/elasticsearch     

### Insert data into elasticsearch
     $ curl -H "Content-Type:application/json" -XPOST localhost:9200/test/tweet   -d '{"name":"naveen", "job":"developer" , "location":"Phoenix", "age":27}'
     $ curl -H "Content-Type:application/json" -XPOST localhost:9200/test/tweet   -d '{"name":"arun", "job":"consultant" , "location":"texas", "age":30}'
     $ curl -H "Content-Type:application/json" -XPOST localhost:9200/test/tweet   -d '{"name":"shiva", "job":"developer" , "location":"chandler", "age":28}'
 

### Run project 
    $ mvn package
    $ mvn exec:java -Dexec.mainClass="com.es.app.ESApp"

