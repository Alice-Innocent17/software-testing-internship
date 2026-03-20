Task 8 - API testing using postman 

OVERVIEW:
This project demonstrates API testing using Postman on public REST APIs. As part of my software testing internship, I performed the four fundamental HTTP methods (GET, POST, PUT, DELETE) to validate CRUD (Create, Read, Update, Delete) operations.The testing was performed on JSONPlaceholder - a free fake API for testing and prototyping.

TECHNOLOGIES USED:
- Postman
- JSONPlaceholder
- Git/GitHub
Base URL: https://jsonplaceholder.typicode.com

TEST EXECUTION:
1. GET request:
   Objective: Retrieve existing user data from the server.
   Expected Result:
       - Status Code: 200 OK
       - Response body contains user details (id, name, email, etc.)
   Actual Result: Passed

2. POST request:
   Objective: Create a new user by sending data to the server.
   Expected Result:
       - Status Code: 201 Created
       - Response includes the sent data plus a new ID
   Actual Result: Passed

3. PUT request:
   Objective: Update an existing user's information.
   Expected Result:
       - Status Code: 200 OK
       - Response shows the updated data
   Actual Result: Passed

4. DELETE request:
   Objective: Remove an existing user from the system.  
   Expected Result:
       - Status Code: 200 OK 
       - Empty response body
   Actual Result: Passed

COLLECTION EXPORT:
The complete Postman collection containing all four requests has been exported and is included in this repository.
File: API-Testing-Collection.postman_collection.json
