# sqlite3-tutorial

```
$ sqlite3 test.db


ls -ptlr - will show the test.db created.

## Reading from external file

.read batch_file.sql


sqlite> CREATE TABLE DEPARTMENT(
   ID INT PRIMARY KEY      NOT NULL,
   DEPT           CHAR(50) NOT NULL,
   EMP_ID         INT      NOT NULL
);



sqlite> .schema


sqlite>.tables
COMPANY     DEPARTMENT

sqlite>.schema DEPARTMENT



sqlite>DROP TABLE COMPANY;



INSERT INTO COMPANY (ID,NAME,AGE,ADDRESS,SALARY)
VALUES (1, 'Paul', 32, 'California', 20000.00 );

INSERT INTO COMPANY (ID,NAME,AGE,ADDRESS,SALARY)
VALUES (2, 'Allen', 25, 'Texas', 15000.00 );

INSERT INTO COMPANY (ID,NAME,AGE,ADDRESS,SALARY)
VALUES (3, 'Teddy', 23, 'Norway', 20000.00 );

sqlite> CREATE TABLE ZACKS_SNP(
   ID INTEGER PRIMARY KEY AUTOINCREMENT,
   Date           CHAR(50) NOT NULL,
   StockName      CHAR(50) NOT NULL,
   StockSymbol    CHAR(50) NOT NULL,
   StockPrice     REAL,
   StockRank      CHAR(50) NOT NULL
);

INSERT INTO ZACKS_SNP (Date,StockName, StockSymbol, StockPrice, StockRank) Values ( "28/3/2023","Zimmer Biomet - ZBH","ZBH",   126.00 ,"BUY");

results.sql

1,$s/^/INSERT INTO ZACKS_SNP (Date,StockName, StockSymbol, StockPrice, StockRank) Values (/g

1,$s/$/);/g

Data Types
1	NULL The value is a NULL value.

2	 INTEGER The value is a signed integer, stored in 1, 2, 3, 4, 6, or 8 bytes depending on the magnitude of the value.

3	REAL The value is a floating point value, stored as an 8-byte IEEE floating point number.

4	TEXT The value is a text string, stored using the database encoding (UTF-8, UTF-16BE or UTF-16LE)

5	BLOB The value is a blob of data, stored exactly as it was input.


Date and Time Datatype

1	TEXT A date in a format like "YYYY-MM-DD HH:MM:SS.SSS"
```
