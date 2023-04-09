# jdbc
## RDBMS - Codd's 12 rule
Java DB Connectivity: API for client-side access to DB, the latest spec is defined in JSR 221
- Has Universal Data Access
- Swappable
Basic Flow of Operation: Mount Driver -> Create connection -> Execute SQL statement -> commit/rollback -> Close connection
JDBC operations throw SQLException

Connections:
- DriverManager: class that interacts with driver to create connection 
- DataSource: interacts with driver for creating connections
- Connection: A class that the developer interacts with that manages the actual communication between the client and the server.
- Statement: rep SQL to be executed against DB
- ResultSet: response from DB in a logical tabular form - values are accessed either by column name or index
- PreparedStatement: an extension of statement that is used for precompiled statement 
- CallableStatement: an extension of PreparedStatement that references stored procedure

Transactions: 
- auto-commit: a function of db driver where each statement is immediately readable by all processes once executed in the RDBMS
- transaction: series of statements that must be executed completely or not at all.
- Rollback: a mechanism by which all statement of a transaction are removed from DB

PostgreSQL: Free and open-source software (FOSS)
- ACID compliant and transactional: ACID is an acronym that stands for Atomicity, Consistency, Isolation, and Durability. It is a set of properties that guarantee that database transactions are processed reliably in a relational database management system (RDBMS). 

Connection pooling: kinda cache connection
ORM - Object Relational mapping | JPA - Java Persistence API | Sprint Data Access pattern
