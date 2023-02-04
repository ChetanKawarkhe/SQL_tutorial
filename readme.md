# Application
  Application is a set of programs to do a particular task

---

### Standalone application
  - Installation is mandatory.
  - Internet is not required.
  - Browswer is not requried/
  - Stored in own device.
  e.g. => notepad, paint, word, excel, temple run etc.
---

### Web application
  - Installation is not mandatory.
  - Internet is required.
  - Browswer is required. 
  - Stored in server.
  e.g. => facebook, instagram, whatsapp, gmail, amazon etc.
--------------------------------------------------------------------

### Client-server application/ mobile application.
  - installation is mandatory.
  - Internet is required.
  - Browswer is required.
  - Stored in server and in own device.
  e.g. => facebook, telegram, instagram, amazon, gmail, pubg etc.
---

### SQL (structured query langugage)
  - SQL is also called as <br/> 
  S - Simple               <br/> 
  E - English             <br/> 
  SQL - Querry            <br/>
  L - Language             <br/> 

### Data
  It is a raw fact which describes attributes of an entity.
  (Attributes = properties)
  (Entity = living / non-living thing / object)

### Database
  Database is a place or medium which is used top store the data in systematic and organised manner.

On database we can perform CRUD operations: 
  * Create / Insert
  * Read / Retreive
  * Update / Modifty
  * Drop / Delete
---


### (DBMS) Database Management System.
  DBMS is a software which is used to maintain and manage the database.

  * In DBMS we can store the data in file format.
  * Here we are using Querry Langugage (QL) to interact with (DBMS).
  * Security and Authorization are the important features of DBMS.

### Security: No third party can acces it. 
Authorization: is giving permission and take back the given permissin.

### RDBMS (Relational DBMS)
  RDBMS is a software which is used to maintain and manage the database.
  * In RDBMS we can store the data in table form.
  * Here we are using structured query language to interact with RDBMS.
  * Security and authorization are two important features.
---

## ***02/02/2023***

### Stucture of table
  * Columns
  => The veritcal sectors in the table is known as columns.

  * Rows
  => The horizontal sectors in the table is known as rows.

  * Cell
  => The smallest unit in the table.
       or
  => The intersection of rows & columns is called as cell.

  * Table
  => The organisation of rows and coolumns is called as table.
  -----------------------------------------------------------------

### Relational Model
  - The data scientist called E.F.Codd invented ralational model.
  - Any DBMS software which follows relational model in it is called becomes RDBMS.
  - In relational model we will store everything in the form of table.
  - DBMS + RN = RDBMS

#### Rules of E.F.Codd 
  1) The data entered in the cell should be a single values data (atomic data).
  2) In RDBMS we can store everthing in the form of tables including metadata. 
    metadata =>  the data about the data is called as metadata and it is stored in metadata. 
    for example:  time, size, date, format of image present in table. 
    this metadata is stores in metatable.
    metadata is created by software.
  3) In RDBNS we can store the data in multiple tables if we want we can create the connection between the tables by using 
     the "Key Attributers"
  4) The data entered in the table can be validated in 2 steps:
     a) By assigning Datatype (mandatory).
     b) By assigning contraints (optional). 
     ![](.\img\1.jpg)
     ![](.\img\2.jpg)
---
## ***03/02/2023***

### Data Types
#### Datatypes are used to find what kind of is present in a particular column.

####  Types:
    1) Char datatype
    2) Varchar/Varchar2 datatype
    3) Date datatype
    4) Number datatype
    5) Large Object
       a) Character large object (LOB)
       b) Binary large object (BLOB)

####  1) Char datatype:
  - It will accept A-Z, a-z, 0-9, '!@#$%^&', '!@#abc'
  - whenever we use char datatype we want ot mention size for it.
  - we can store upto 2000 memory allocation
  - char uses "fixed length memory allocation".
  - syntax = Chhar(size)

  - it uses fixed length memory allocation. 
  - we  have to define the length first.
  - it can lead to memory wastage.
  ![](.\img\3.jpg)

#### 2)Varchar: 
   - It will accept 'A'to 'Z', 'a't 'z', 0 to 0, '!@#$%^&', '!@#abc'.
   - whenever we use varchar datatype we want to mention some size for it.
   - we can store upto 2000 memory allocation.
   - varchar uses "variable length memory allocation".
   - Syntax = VARCHAR(size)
   - unused memory will be used for other data,. (no memory wastage.)

#### Varchar2:
  - It is an updated version of varchar
  - we can store upto 4000 memory allocation\
  - syntax = varchar2(size)

#### 3) Date:
  - it is used to store the data in a particular date format.
  - syntax = Date

  ##### oracle date formats:
    a) DD-MON-YYYY eg.=> '10-NOV-2023'
    b) DD-MON-YY    eg.=> '10-NOV-23'

#### 4) NUMBER datatype:
   - it is used  to store numerical values.
   - syntax = Number(Precision[,scale])

   eg. 999.99    
   where 999 is precesion and .99 is scale.

   * Precision
     - Precision is nothing but interger values.
     - Precision cant be 0
     - Precision ranges from 1 to 38
     - There is no default value for precision

   * Scale
     - Scale is nothing but decimal values
     - The default value of scale is 0.
     - scale ranges from -84 to 127

## 04/02/2023
#### `5) Large Object:-`
  a) Character large object:    
    - It is used to store the Binary value of image, mp4, mp3, document .....upto 4GB size.   
    - Syntax: ```CLOB```
  
  b) Binary large object :    
    - It is used to store the binary value of image, mp4, mp3, document ....upto 4GB of size.   
    - Syntax: ```BLOB```

---

## `Constraints`
  - Constraints are the extra validation given for a particular column.
 ### Types:
  1) Unique constraint
  2) Not Null constraint
  3) Check constraint
  4) Primary key
  5) Foreign key

### `1) Unique constraint:`
  - Unique is a constraint in which it will not accept repeated and duplicate values.

### `2) Not Null constraint:`
  - Not Null is a constraint in which it will not accept null values. 
    #### Notes:-
    - Null means empty or nothing.
    - 0 is not a null value.
    - Any operations that can be performed with Null becomes Null.
    - eg.:-
      - 1 + Null = Null
      - 1 - Null = Null
      - 1 * Null = Null
      - 1 / Null = Null

### `3) Check constraint:`
  - Check is the constraint in which it will be given as extra validation depending upon the condition, if the condition is true it will accept the values else it will reject.

  - eg.:-
    - 1) check (SAL > 0)
    - 2) check (LENGTH(PH_No) = 10)
  
### `4) Primary Key:-`
  - Primary key is a constraint which  is used to identify the record uniquely from the table characteristics of primary key.
  - Primary key will not accept duplicate and repeated values.
  - Primary key will not accept Null values.
  - Primary key is a combination of unique and Not Null.
  - Primary key is not mandatory but recommended to have one in an table.
  
### `5) Foreign Key:-`
```diff
+Foreign key is used to create connection between multiple table characteristics of foreign key.
+Foreign key will accept repreated and duplicate values.
+Foreign key will accept Null values.
  - To be a foreign key it should be the primary key in its own table.
  - Actually foreign key is present in child table but belong to parents table.
  - foregin key is also called as 'Referential integrity constraint'.
-Foreign key is not a combination of Unique and Not Null.
```
![](.\img\4.jpg)

---