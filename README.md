# cassandra_docker-compose
 ## Running cassandra as docker compose

Cassandra database was run with docker compose in the file with yml extension in the file.
The terminal screen shot of the database being run is also among the files.

The source I used during this process: [link](https://citizix.com/how-to-run-cassandra-4-with-docker-and-docker-compose/)


## Which databases does Instagram use?

[![Alt text](https://miro.medium.com/v2/resize:fit:1400/0*nZeSkWrur4Ne6NH4.png "Instagram Structure")](https://interviewnoodle.com/instagram-system-architecture-fdbec22e48ee)

As seen in the image, Instagram uses Redis and Cassandra as its database.

## Why does Instagram use Cassandra?

Cassandra is a high performance and highly scalable distributed open source NoSQL database management system. [1](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwiexPy35oqDAxVjQfEDHfZaAvcQFnoECBIQAw&url=https%3A%2F%2Fwww.geeksforgeeks.org%2Fdifference-between-cassandra-and-rdbms%2F%23%3A~%3Atext%3DCassandra%2520is%2520a%2520high%2520performance%2CCassandra%2520is%2520a%2520NoSQL%2520database.&usg=AOvVaw3IdkhZ6kmcjnQFO6f5tpKE&opi=89978449) It is a decentralized, scalable storage system designed to handle vast volumes of data across multiple commodity servers, providing high availability without a single point of failure. [2](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwiexPy35oqDAxVjQfEDHfZaAvcQFnoECAwQAw&url=https%3A%2F%2Fwww.spiceworks.com%2Ftech%2Fbig-data%2Farticles%2Fwhat-is-cassandra%2F%23%3A~%3Atext%3DCassandra%2520is%2520an%2520open%252Dsource%2520NoSQL%2520distributed%2520database%2520that%2520manages%2Ca%2520single%2520point%2520of%2520failure.&usg=AOvVaw1bJlOTT2SVa5JcFrA4pf4M&opi=89978449) Instagram uses Cassandra as a general key-value storage service, to support the user photo feed, direct messages, as well as for fraud detection. [3](https://thenewstack.io/instagram-supercharges-cassandra-pluggable-rocksdb-storage-engine/#:~:text=Instagram%20uses%20Cassandra%20as%20a,in%20slow%20performance%20for%20users.)

With this information I found from various sources, I think that Instagram has chosen a decentralized structure due to high-scale data storage. Moreover, due to the key-value structure, the accounts to which data such as photos and comments belong will be more easily identified.
