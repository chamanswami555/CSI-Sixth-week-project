Test API using Postman
First Create a New POST Request 
Then put URL  : http://localhost:8000/api/user/create
Then choose Body -> raw ->json 
And Write the json of name, email and address
{
   “name”:”John”,
   “email”:”john@gmail.com”,
   “address”:”Canada”
}
Now just press on Send and see the Body there is same json 
postman
Now check the database you will see the data in users collection. 

data inserted into database
Now Let’s test the GET API endpoint for getting all data from database 

For that, Just select GET method and provide the URL  http://localhost:8000/api/user/getAllUsers

getting all data from databse
Now let’s update data from database using PUT method provide URL 

First Create a New PUT Request 
Then put URL  : http://localhost:8000/api/user/update/id
Then choose Body -> raw ->json 
And Write the json of name, email and address
{
   “name”:”John Doe”,
   “email”:”john123@gmail.com”,
   “address”:”USA”
}
Now just press on Send and see the Body there is same json 
put method to update data from database
Now For deleting data from data you can just add the new DELETE request and API endpoint : http://localhost:8000/api/user/delete/id

delete user by id
If data is deleted successfully. It will show the message 
{“message “: “User deleted successfully”}
