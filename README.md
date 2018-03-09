# Python-mysql
import pymysql  #导入pymysql库

db = pymysql.connect("127.0.0.1","root","root","data_test" )  #打开数据库连接

cursor = db.cursor()  #使用 cursor() 方法创建一个游标对象 cursor 

sql1 ="CREATE TABLE Writers(Id INT PRIMARY KEY AUTO_INCREMENT, Name VARCHAR(25))"

cursor.execute(sql1)  #创建一个表 
