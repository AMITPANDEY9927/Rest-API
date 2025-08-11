# Rest-API
Flask User Management API

Overview
This is a simple RESTful API built with Flask for managing user data. It supports CRUD operations (Create, Read, Update, Delete) using an in-memory dictionary as the data store.

Features

GET /users → Retrieve all users

GET /users/<user_id> → Retrieve a single user by ID

POST /users → Create a new user

PUT /users/<user_id> → Update an existing user

DELETE /users/<user_id> → Delete a user

Requirements

Python 3.x

Flask

Installation

Clone this repository or copy the script.

Install Flask: pip install flask

Run the application: python app.py

API Endpoints

Get All Users
Request: GET /users
Response: {"1": {"id": 1, "name": "John"}}

Get User by ID
Request: GET /users/1
Response (200 OK): {"id": 1, "name": "John"}
Response (404 Not Found): {"error": "User not found"}

Create a User
Request: POST /users
Body: {"name": "Alice"}
Response (201 Created): {"id": 2, "name": "Alice"}

Update a User
Request: PUT /users/1
Body: {"name": "Mike"}
Response (200 OK): {"id": 1, "name": "Mike"}

Delete a User
Request: DELETE /users/1
Response (200 OK): {"message": "User deleted"}

