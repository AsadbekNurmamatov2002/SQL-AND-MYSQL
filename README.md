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
ma'lumot Kiritish - __INSERT INTO__
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/b61c60ec-c816-4591-b2ce-64740e5e0714)
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/fc97a625-a87c-40a5-ab83-135869f77ec4)

ma'lumot chiqarish - __SELECT * FROM table_name;__
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/ac929a0b-ea5e-40df-b2cf-b52b31655dec)
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/defd02a6-fdd5-4f2d-974b-e227dee830aa)


# Mysql- WHERE 
>
__SELECT column1, column2, ...
FROM table_name
WHERE condition;__
>
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/772affc2-19e7-48c7-bcb7-b0c6d7b35c67)
__Chizilgan chiziq boylab Jajvaldan ma'lumot 
>      SELECT*FROM table_name WHERE ism='Suhrob' ;
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/d0bf246a-2f2c-491c-9569-929e92beabea)
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/740af3c4-c0e5-4aec-8e52-42461bf31f74)
__Chizilgan chiziq boylab Jajvaldan ma'lumot olish__
>      SELECT id , ism, familya, telefon FROM table_name WHERE familya='Nurmamatov' ;
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/3a282bf0-cd28-4d2f-821b-c5092f026ce9)

#Mysql - WHER ->AND , OR va NOT
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/23e36af2-f260-47a0-a848-fc909206b043)
__SELECT ustun1, ustun2, ...
FROM table_name
WHERE  holat1 OR holat2 OR holat3 ...;__
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/85197ee7-ad64-4ea0-9d21-7456007f2fb7)

__SELECT ustun1, ustun2, ...
FROM table_name
WHERE NOT holat;__
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/fad18b66-ef94-407d-8949-9d63207129b2)

# Mysql-ORDER BY, DESC, ASC
__familya__ ustun bo'yicha tartiblash
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/e7186c68-5a34-4c46-baab-a3493f5de1ba)
__familya__ ustun bo'yicha kamiyish Tartibida tartiblash
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/b9678486-2811-46a4-be55-d8db654c5f11)
__familya__ ustun bo'yicha o'shish bo'yicha tartiblaydi
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/31d5d769-3f30-4dfa-853c-cae7713132e8)
__ASC+DESC__
ism ustun bo'yicha o'shish, familya bo'yicha kamiyish tartibida joylashtiradi
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/43717473-c0c0-4754-8756-327b16998596)
#Mysql-LIMIT
__SELECT ustun(s)
FROM table_name
WHERE holat
LIMIT number;__
>__LIMIT__ - CHIKLOV
code-> __SELECT*FROM table_name WHERE shahar="Samarqand" LIMIT 2;__
shahar ustun bo'yicha 2 ta smarqand nomli satrlarni olish
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/38d82e5d-bb53-4201-bbda-5b07793fae20)

__MySQL MIN() va MAX() funksiyalari__
-Funktsiya MIN()tanlangan ustunning eng kichik qiymatini qaytaradi.

-Funktsiya MAX()tanlangan ustunning eng katta qiymatini qaytaradi.
## MIN()-ishlatilishi
>
__SELECT MIN(ustun)
FROM table_name
WHERE holat;__
>
bu jadvaldan eng kichik telifon numberni topish(misol uchun)
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/0a52f865-ac5d-43a2-9344-22bea1a93564)
code-> __SELECT MIN(telefon) FROM table_name ;__ 
etibor bering (table_name) bu biz boshlanggich darsda jadval nomini -> __table_name__ deb bergandek
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/25183d8e-d849-4df4-887b-5efb011abddc)
__AS__ -orqli biz jadval nomini uzgartirishimiz mumkun
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/4eff5abd-0570-40c9-9b19-2ae3b12d8d5f)
## MAX()-ishlatilishi
__SELECT MAX(ustun)
FROM table_name
WHERE holat;__
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/1b469031-982d-42a1-97c5-987df18315a3)

__MySQL COUNT(), AVG() va SUM() funksiyalari__
__COUNT()__ - funksiyasi (sonini aniqlaydi) O'xshash holatlar sonini aniqlaydi
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/d470e3a1-24cb-4728-9e2c-bc12ad1ebc0b)
__AVG()__Funktsiya raqamli ustunning o'rtacha qiymatini qaytaradi. 
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/d39f1c34-070c-4762-ac46-e7b36d4c519f)
__ SUM()__Funktsiya raqamli ustunning umumiy yig'indisini qaytaradi. 
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/75ea99a3-ba06-4019-b373-a009d196cd11)
__MySQL LIKE operatori__
Ustun ichida belgilangan naqshni qidirish uchun operator LIKEbandda ishlatiladi 
LIKE "a%"-> a va A bilan boshlanovshi qiymatlarni ob beradi
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/7853bcbf-af08-42c5-ae29-8bc98c1a17a6)
LIKE "%n"-> n va N bilan tugavchi qiymatlarni oladi
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/55c74f4c-6303-4cf9-9bd4-017244935add)

__MySQL IN operatori__
-Operator INbandda bir nechta qiymatlarni belgilash imkonini beradi.
__SELECT ustun_name(s)
FROM table_name
WHERE ustun_name IN (value1, value2, ...);__
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/c00f4ff8-d8cb-4e59-8886-4a658ac5d72b)

__MySQL BETWEEN operatori__
-Operator BETWEENma'lum diapazondagi qiymatlarni tanlaydi. Qiymatlar raqamlar, matn yoki sana bo'lishi mumkin.
-Operator BETWEEN o'z ichiga oladi: boshlang'ich va tugatish qiymatlari kiritilgan.
__SELECT column_name(s)
FROM table_name
WHERE column_name BETWEEN value1 AND value2;__
-__BETWEEN va NOT BETWEEN__
-__ORASIDA va __ORASIDA EMAS__- qo'llanilishi
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/981ad3c9-1f5c-4618-ad7b-e8693a7a7f94)

# MySQL ulanishlari
Ikki yoki undan ortiq jadvallar qatorlarini ular orasidagi tegishli ustun asosida birlashtirish uchun __JOIN__ ishlatiladi .
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/38a06039-e69a-4332-8d59-598cea56e46e)
iNNER JOIN
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/9fc3a833-ce60-4a50-9ed1-ae2a7321bafe)

LEFT JOIN
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/fc87e3a1-6618-4ae1-944d-b053a90c98e1)
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/d9667177-7b47-4730-ab85-a4bd875e4777)

RIGT JOIN
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/de3b0def-6587-4fa2-91cc-e2f538625bb8)
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/d0c77797-c434-44e3-8fbf-74362ab099c7)
UNION JOIN
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/af29728c-c504-4ec8-b84e-a0577a8a7d3b)
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/8d2f54e5-f1d6-4984-ad97-5251ff544aa0)
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/6a305ae7-2223-483b-91d5-e1880ef38821)
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/83787eaa-dc2c-4644-8654-94249bb3e928)
![image](https://github.com/AsadbekNurmamatov2002/SQL-AND-MYSQL/assets/144318530/f471e593-30c9-456b-8989-e429121edb83)






