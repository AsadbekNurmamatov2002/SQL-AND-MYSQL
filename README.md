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
>
>                                         SQL- STRING datatype
>            Data type	          Ish bajarishi
             CHAR(size)	         |SATILGAN uzunlikdagi satr (harflar, raqamlar va maxsus belgilarni o'z ichiga olishi mumkin). Size parametri ustun uzunligini belgilar bilan belgilaydi - 0 dan 255 gacha bo'lishi mumkin. Standart 1
             VARCHAR(size)       |VARIABLE uzunlikdagi satr (harflar, raqamlar va maxsus belgilarni o'z ichiga olishi mumkin). Size parametri belgilarda maksimal satr uzunligini belgilaydi - 0 dan 65535 gacha bo'lishi mumkin
             BINARY(size)        |CHAR() ga teng, lekin ikkilik bayt satrlarini saqlaydi. Size parametri baytlarda ustun uzunligini belgilaydi. Standart 1
             VARBINARY(size)	   |VARCHAR() ga teng, lekin ikkilik bayt satrlarini saqlaydi. Size parametri baytlardagi maksimal ustun uzunligini belgilaydi.
             TINYBLOB	           |BLOBlar uchun (ikkilik katta ob'ektlar). Maksimal uzunlik: 255 bayt
             TINYTEXT	           |Maksimal uzunligi 255 belgidan iborat bo'lgan qatorni ushlab turadi
             TEXT(size)	         |Maksimal uzunligi 65 535 bayt bo'lgan satrni ushlab turadi
             BLOB(size)	         |BLOBlar uchun (ikkilik katta ob'ektlar). 65 535 baytgacha ma'lumotga ega
             MEDIUMTEXT          |Maksimal uzunligi 16 777 215 belgidan iborat bo'lgan satrni ushlab turadi
             MEDIUMBLOB          |BLOBlar uchun (ikkilik katta ob'ektlar). 16 777 215 baytgacha ma'lumotni saqlaydi
             LONGTEXT	           |Maksimal uzunligi 4,294,967,295 belgidan iborat bo'lgan satrni ushlab turadi
             LONGBLOB	           |BLOBlar uchun (ikkilik katta ob'ektlar). 4 294 967 295 baytgacha maʼlumotga ega
             ENUM(val1, val2, ...) |Mumkin bo'lgan qiymatlar ro'yxatidan tanlangan, faqat bitta qiymatga ega bo'lishi mumkin bo'lgan satr ob'ekti. ENUM ro'yxatida 65535 tagacha qiymatlarni sanab o'tishingiz mumkin. Agar ro'yxatda bo'lmagan qiymat kiritilsa, bo'sh qiymat kiritiladi. Qiymatlar siz kiritgan tartibda tartiblanadi
             SET(val1, val2, ...)|Mumkin boʻlgan qiymatlar roʻyxatidan tanlangan 0 yoki undan ortiq qiymatga ega boʻlishi mumkin boʻlgan satr obyekti. Siz SET ro'yxatida 64 tagacha qiymatni sanab o'tishingiz mumkin



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

# MySql darslar
## 1-dars
### Mysql-install
Bu site ga kiring __https://dev.mysql.com/downloads/installer/__
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/aae2af50-2e3a-4819-8196-a9d12d1d20b3)
bu-pastagi tugmani bosing
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/747475d6-dba7-4a73-8cba-4129867971ca)
va kiyingi sahifaga o'ting
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/fc917729-575f-4f2d-9a67-4486f7ddfa88)
kiyin bu tugmani bosing 
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/f30817ef-9e75-45c0-a1c2-e7ef3f79631e)

__MySql-DATA-TYPE__
>CHAR(size)-Size parametri ustun uzunligini belgilar bilan belgilaydi - 0 dan 255 gacha bo'lishi mumkin. Standart 1
>VARCHAR(size)-harflar, raqamlar va maxsus belgilarni o'z ichiga olishi mumkin. Hajmi parametri maksimal ustun  - 0 dan 65535 gacha bo'lishi mumkin
>BINARY(size)-CHAR() ga teng, lekin ikkilik bayt satrlarini saqlaydi. Size parametri baytlarda ustun yordamni olish. Standart 1

1-qadam  
>    windows+R
tugmani bosim __cmd__ kiriting
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/77e28755-c71d-4cd6-afdd-c82d2f837da8)

![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/7ff85a4f-9ebf-4837-9536-d24c42a527e6)

![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/24f7c1dd-ac71-4529-bd87-1513920425b5)

![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/ad3ed256-2fd4-4d3b-8030-cb88bc0f8b6a)

![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/46f7c614-227a-43e2-9833-3a462198f86e)

![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/167867c3-78f3-4f65-96fe-9092a868c38a)

![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/e49c6a7f-8987-4f55-b6b6-55adc5b5300d)

![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/7bd58050-9ec6-4e34-8c13-ff08c8db41d2)


![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/71dafe25-97ff-49ba-8dea-aee6e7494acc)

![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/b61c60ec-c816-4591-b2ce-64740e5e0714)

![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/ac929a0b-ea5e-40df-b2cf-b52b31655dec)





