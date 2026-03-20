Task 8 - API testing using postman 

OVERVIEW:
This project demonstrates API testing using Postman on public REST APIs. As part of my software testing internship, I performed the four fundamental HTTP methods (GET, POST, PUT, DELETE) to validate CRUD (Create, Read, Update, Delete) operations.The testing was performed on JSONPlaceholder - a free fake API for testing and prototyping.

TECHNOLOGIES USED:
Tool	           |   Purpose
Postman	         |   API testing client
JSONPlaceholder	 |   Free fake API for testing
Git/GitHub	     |   Version control and submission

API ENDPOINTS TESTED:
Method	 |   Endpoint	 |   Description
GET	     |   /users/2	 |   Retrieve user with ID 2
POST	   |   /users	   |   Create a new user
PUT	     |   /users/1	 |   Update existing user with ID 1
DELETE	 |   /users/1	 |   Delete user with ID 1
Base URL: https://jsonplaceholder.typicode.com

TEST EXECUTION:
1. GET request:
   Objective: Retrieve existing user data from the server.
   Request Details:
   - Method: GET
   - URL: https://jsonplaceholder.typicode.com/users/2
   Expected Result:
   - Status Code: 200 OK
   - Response body contains user details (id, name, email, etc.)
   Actual Result: Passed

2. POST request:
   Objective: Create a new user by sending data to the server.
   Request Details:
   - Method: POST
   - URL: https://jsonplaceholder.typicode.com/users
   - Headers: Content-Type: application/json
   - Request Body:
          {
            "name": "John Wick",
            "username": "johnwick",
            "email": "john@continental.com",
            "phone": "555-123-4567",
            "website": "continental.com"
           }
   Expected Result:
   - Status Code: 201 Created
   - Response includes the sent data plus a new ID
   Actual Result: Passed

3. PUT request:
   Objective: Update an existing user's information.
   Request Details:
   - Method: PUT
   - URL: https://jsonplaceholder.typicode.com/users/1
   - Headers: Content-Type: application/json
   - Request Body:
          {
            "id": 1,
            "name": "Leanne Graham Updated",
            "username": "Bret",
            "email": "Leanne@updated.com",
            "phone": "1-770-736-8031 x56442",
            "website": "updated.org"
           }
   Expected Result:
   - Status Code: 200 OK
   - Response shows the updated data
   Actual Result: Passed

4. DELETE request:
   Objective: Remove an existing user from the system.
   Request Details:
   - Method: DELETE
   - URL: https://jsonplaceholder.typicode.com/users/1
   Expected Result:
   - Status Code: 200 OK 
   - Empty response body
   Actual Result: Passed

COLLECTION EXPORT:
The complete Postman collection containing all four requests has been exported and is included in this repository.
File: API-Testing-Collection.postman_collection.json
