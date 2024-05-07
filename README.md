# rookie-db
Conventional database management system (DBMS) enhanced through the integration of B+tree indexing, efficient sort, hash, and join algorithms, and optimized query reordering and optimization, similar to IBM System R. Implemented transaction concurrency through a lock manager that supports locking at both coarse and fine granularities.

This is a very large project build over months. The most relevant code samples exist in the following files:
- Trees and Indexing:
    - src/main/java/edu/berkeley/cs186/database/index/BPlusTree.java
    - src/main/java/edu/berkeley/cs186/database/index/InnerNode.java
    - src/main/java/edu/berkeley/cs186/database/index/LeafNode.java
