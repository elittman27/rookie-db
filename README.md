# rookie-db
Conventional database management system (DBMS) enhanced through the integration of B+tree indexing, efficient sort, hash, and join algorithms, and optimized query reordering and optimization, similar to IBM System R. Implemented transaction concurrency through a lock manager that supports locking at both coarse and fine granularities.

This is a very large project build over months. The most relevant code samples exist in the following files:
- Trees and Indexing:
    - src/main/java/edu/berkeley/cs186/database/index/BPlusTree.java
    - src/main/java/edu/berkeley/cs186/database/index/InnerNode.java
    - src/main/java/edu/berkeley/cs186/database/index/LeafNode.java
- Query optimization, Sorting, and Hashing:
    - src/main/java/edu/berkeley/cs186/database/query/join/BNLJOperator.java
    - src/main/java/edu/berkeley/cs186/database/query/join/SortOperator.java
    - src/main/java/edu/berkeley/cs186/database/query/join/SortMergeOperator.java
    - src/main/java/edu/berkeley/cs186/database/query/join/GHJOperator.java
    - src/main/java/edu/berkeley/cs186/database/query/QueryPlan.java
- Concurrency:
    - src/main/java/edu/berkeley/cs186/database/concurrency/LockType.java
    - src/main/java/edu/berkeley/cs186/database/concurrency/LockManager.java
    - src/main/java/edu/berkeley/cs186/database/concurrency/LockContext.java
    - src/main/java/edu/berkeley/cs186/database/concurrency/LockUtil.java
    - src/main/java/edu/berkeley/cs186/database/table/Table.java
    - src/main/java/edu/berkeley/cs186/database/table/PageDirectory.java
    - src/main/java/edu/berkeley/cs186/database/memory/Page.java
    - src/main/java/edu/berkeley/cs186/database/Database.java
- Recovery:
    - src/main/java/edu/berkeley/cs186/database/recovery/ARIESRecoveryManager.java
