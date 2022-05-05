# Shilpa
import mysql.connector 

mydb=mysql.connector.connect(host="localhost",user="root",passwd="",database="shilpa")

mycursor =mydb.cursor()

mycursor.execute("select * from movie")

for i in mycursor:
    print(i)
