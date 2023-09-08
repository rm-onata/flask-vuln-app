## sql injection
 
 
###### This vulnerability can be exploited to dump the contents of an applications database.
###### The most popular database is MySQL but you will run into others such as MSSQL, PostgreSQL, Oracle, and more.
 
 ```python
user_supplied_input = requests.get("user_supplied_input")
query = "select id from vuln_table where vuln = " + user_supplied_input
cursor = db.cursor()
cursor.execute(query, (ip,))
result = cursor.fetchall()
cursor.close()
 ```
 
 
