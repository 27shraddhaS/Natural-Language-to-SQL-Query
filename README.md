# Natural-Language-to-SQL-Query
Converting a natural language sentence to an SQL query using NLP and LSTM

# Working
Enter a question regarding the database in english language. The 'Convert' button runs this sentence through 
NLP parser -> network of decision making clauses -> LSTM models -> return the converted SQL query.

The 'Execute' button will execute this generated query, fetch the result from the MySQL database and display the table to the user.

![nl-sql.png](nl-sql.png)

# Example

### User question:
show airports in france

### Converted SQL query:
SELECT airport FROM flight WHERE country = "france" ;

### User question:
Create view v1 that show songs of singer taylor swift

### Converted SQL query:
CREATE VIEW [v1] AS SELECT songs FROM singer WHERE name = "taylor swift";

### User question:
give the singers from india

### Converted SQL query:
SELECT * FROM singer WHERE country = "india" ;
