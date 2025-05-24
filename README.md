**User Management RESTful Microservice using Spring Boot**

This microservice is designed to handle basic user-related operations in a RESTful manner. It leverages Spring Boot to expose HTTP endpoints for creating, retrieving, and deleting user records.

**Key Features:**

**1. Retrieve All Users**

Endpoint: GET /users

Description: Returns a list of all registered users.

Response: JSON array contains user objects with fields like id, name, and birthDate.

![image](https://github.com/user-attachments/assets/060ed3eb-1584-4b6a-bd33-6dd2cdde2061)


**2. Retrieve a User by ID**

Endpoint: GET /users/{id}

Description: Returns the details of a specific user by their unique ID.

Response: JSON object representing the user.

![image](https://github.com/user-attachments/assets/e9ed80ae-6b62-43c6-91b1-90e53e4736fa)

Error Handling: Returns a 404 Not Found if the user with the given ID does not exist.

![image](https://github.com/user-attachments/assets/9286ff93-6154-4cb6-a17d-7cf32a902cd5)


**3. Create a New User**

Endpoint: POST /users

Description: Accepts user data (e.g., name, birthDate) in the request body and stores it.

Request Body: JSON object with required fields.

{

  "name": "John Doe",
  
  "birthDate": "1990-05-24"
  
}

Response: Returns the created user object with a generated ID and a 201 Created status.

![image](https://github.com/user-attachments/assets/694dae49-2966-43c0-afc8-c894fa09edc1)


**4. Delete a User by ID**

Endpoint: DELETE /users/{id}

Description: Deletes a user with the specified ID.

Response: Returns 200 No Content on successful deletion.

![image](https://github.com/user-attachments/assets/bd511147-df37-48ac-a630-56364c0ee6ab)
