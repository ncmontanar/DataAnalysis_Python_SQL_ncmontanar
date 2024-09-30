##### from https://github.com/ankitbansal6/data_analytics_project
1) 
1.1. Get the kaggle token
1.2. get the DBB url (ankitbansal06/retail-orders)
https://github.com/ankitbansal6/data_analytics_project/blob/main/sql_code.sql

---
2)   
**import libraries**

`pip install kaggle` 

**import DBB (dwnload from kaggle)**

`kaggle datasets download ankitbansal06/retail-orders -f orders.csv`    

**unzipp the DBB zip**
(in ipnb)
- Read data from the file and handle null values

`import pandas as pd`
`df.shape`
---
3) 
**Cleanning : **
(in ipnb)
- change the non-values for NaN
- utiliser na_values methode
- fix the colome names (1to1)
- rename nton
- replacer hiphens

---
4) 
**calculate new columns :  discount , sale price and profit**
- Print the column information
- convert order date from object data type to datetime
- convert order date from object data type to datetime (order_date):
- load the data into sql server using replace option

---
5) 
**connect to mysql**
connect to my sqlserver (is : DESKTOP-MT2MGIU  from sqlserver)  i.e. engine = sal.create_engine('mssql://ANKIT\SQLEXPRESS/master?driver=ODBC+DRIVER+17+FOR+SQL+SERVER')
1.on va creer une connection 'engine' et 2. le connector mssql (ou postre ou mysql si nécessaire) et 3. master est la base à la quelle je veux me connecter 
/master?driver=ODBC+DRIVER+17+FOR+SQL+SERVER vient de sqlserver bdd Master :

`pip install pyodbc`
***driver : in windows rechercher : ODBC ***
---
6) 
**Create the schema**
- to  get sharp with the DBB, drop the table, provide the rigth dLL adn change 'append' by 'replace'*/
- load the data into sql server using append option

---
7) almost done :  

    -- find top 10 highest reveue generating products 
    -- find top 5 highest selling products in each region
    -- for each category which month had highest sales 
    -- which sub category had highest growth by profit in 2023 compare to 2022