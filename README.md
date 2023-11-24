![photo_2023-11-23_18-30-21](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/4897b6d8-8b6a-45d4-8aed-dd54d232f5ae)

                                            __ SQL-CREATE DATABASE va CREATE TABLE__
    __CREATE DATABASE__ --Ushbu CREATE DATABASEbayonot yangi SQL ma'lumotlar bazasini yaratish uchun ishlatiladi.
    __CREATE TABLE__--bayonot ma'lumotlar bazasida yangi jadval yaratish uchun ishlatiladi.
>        CREATE DATABASE databasename;

>        CREATE TABLE table_name (
>        column1 datatype, 
>        column2 datatype,
>        column3 datatype,
>       ....
>       );

column-Ustun parametrlari jadval ustunlarining nomlarini belgilaydi.

--Misol--
>         CREATE DATABASE Foydatabases;
>         CREATE TABLE Foydalanovchi (
>         FoydalanovchiID int,
 >        Familya varchar(255),
>         Ism varchar(255),
 >        Address varchar(255),
 >        Shahar varchar(255)
 >       );


                                                             __ SQL - DATA TYPE__
![SQL-DATATYPE](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/d6c42457-5e14-40df-b15e-90dde8f497ef)

                                                             SQL-intager data type 
                                                      SQL- butun sonli ma'lumotlar turi 
                                                                               
>        SQL butun sonli ma'lumotlar turi  ||  Baytlar soni || Qiymatlar diapazoni

>        SMALLINT  ______________________________ 2 ____________ -32767 dan 32767 gacha
>        INTEGER, INT, SERIAL____________________4 ___________ -2,147,483,647 dan 2,147,483,647 gacha
>        INT8, BIGINT, SERIAL8, BIGSERIAL_______ 8____________  -9,223,372,036,854,775,807 dan 9,223,372,036,854,775,807 gacha

                                                CREATE TABLE-misollar
                                                
>                  CREATE TABLE talaba(
>                   id int NOT NULL AUTO_INCRIMINT, ("id AUTOINCREMENT PRIMARY KEY"-__MS Access  uchun__)
>                   ismi VARCHAR(200),
>                   familya VARCHAR(250),
>                    yoshi INT(3),
>                   adres varchar(100),
>                   phone VARCHAR(15) NOT NULL UNIQUE
>                     );
>
>                      _______________________________________________________
 >                    |  id   |   ismi  | familya  | yoshi  | adres  |  phone |
>                      """"""""""""""""""""""""""""""""""""""""""""""""""""""""

> ```
>                                      ### **SQL-JOIN**
> ```
> 
> ![sql-joins](https://user-images.githubusercontent.com/144318530/285369025-e3f3905b-8954-439c-a4b1-e6b027ed3a47.png)
> 
> >                                     misollar:
>                             CREATE TABLE  sqljoin1(
>                             id int NOT NULL  AUTO_INCRIMENT,
>                             firstname VARCHAR(200),
>                             listname VARCHAR(200),
>                             phone INT(15),
>                            );
> 
> ```
>                             CREATE TABLE  sqljoin2(
>                             id int NOT NULL  AUTO_INCRIMENT,
>                             adress VARCHAR(200),
>                             cety VARCHAR(200),
>                             phone INT(15)
> ```
> 
> );
> 
> > ```
> >           ***SQL - INNER JOIN***
> > ```
> > 
> > 
> >     
> >       
> >     
> > 
> >       
> >     
> > 
> >     
> >   
> > SELECT*TABLE  sqlinner1 as A INNER JOIN  sqlinner1 as B ON A.id=B.id;

