NOTE: There's a problem in that the original data has nulls in it, and mongoimport doesn't do well with nulls when the source is CSV. So I'm going to completely redo this and generate BSON files instead. Stay tuned...

# mongodb-classicmodels
MongoDB / CSV version of the ClassicModels sample database.

This came from here:

http://www.mysqltutorial.org/mysql-sample-database.aspx

which in turn likely came from here:

https://www.richardtwatson.com/dm6e/

To import it into mongodb, just run the mongo-import.sh script.

If you want it to go into a different database, edit the mongo-import.sh script and change each occurance of "ClassicModels" to whatever you like.

You can also open the CSV files in Excel or LibreOffice.

I borrowed the bash script from here, which is a really nice implementation of the Northwind database in CSV and Mongo: https://github.com/tmcnab/northwind-mongo
