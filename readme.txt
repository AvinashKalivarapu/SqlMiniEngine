
Build a a mini­sql engine which will run a subset of SQL Queries using ​command line interface with proper error handling 

DATASET :

1) csv files for tables.
    -->If a file is: ​File1.csv,the table name would be File1.
2) Integer elements in files
3) A file named --> metadata.txt​  
   which will have the following structure for each table: 
   <begin_table> 
   <table_name> 
   <attribute1> 
   .... 
 
   <attributeN> 
   <end_table>      


TYPE OF QUERIES:​
  
1)   Select all records : elect * from table_name; 

2)   Aggregate functions: Simple aggregate functions on a single column. Sum, average, max and min. 

3)   Project Columns(could be any number of columns) from one or more tables : Select col1, col2 from table_name;
 
4)   Select/project with distinct from one table : select distinct(col1), distinct(col2) from table_name;
 
5)   Select with where from one or more tables: select col1,col2 from table1,table2 where col1 = 10 AND col2 = 20; 
       --> In the where queries, there can be a maximum of one AND/OR operator with no NOT operators. 
6)   Projection of one or more(including all the columns) from two tables with one join condition :  
        a)   select * from table1, table2 where table1.col1=table2.col2; 
        b)   select col1,col2 from table1,table2 where table1.col1=table2.col2; 
 
FORMAT OF INPUT:

{compiled files} "SQL Query"

Example : ./a.out "select * from table_name where condition"



 
