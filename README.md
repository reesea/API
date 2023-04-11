## Retrieve User Data API Documentation
### Introduction
This API documentation outlines how to retrieve user data from our system using RESTful API calls. The Retrieve User Data API allows you to get user data including their name, email, and other relevant details. This document provides a detailed description of the API's endpoints, parameters, response, and authentication process.

### API Endpoints
This API provides the following API endpoints for developers to use:

* `GET /users` - retrieves user data based on specified parameters
* `POST /users` - creates a new user in the system

### Authentication
The Retrieve User Data API requires authentication through an API key. To obtain an API key, please contact our support team at support@umbili.com.

### Parameters
#### GET /users
* `id` (optional) - retrieves user data based on a specific user ID
* `name` (optional) - retrieves user data based on a specific user name
* `email` (optional) - retrieves user data based on a specific user email

#### POST /users
* `name` (required) - the name of the new user
* `email` (required) - the email of the new user
* `password` (required) - the password of the new user

### Response
#### GET /users
The response from the Retrieve User Data API returns a JSON object with the following fields:

* `id` - the unique ID of the user
* `name` - the name of the user
* `email` - the email of the user
* `created_at` - the date and time the user was created
* `updated_at` - the date and time the user was last updated

#### POST /users
The response from the Retrieve User Data API returns a JSON object with the following fields:

* `id` - the unique ID of the new user
* `name` - the name of the new user
* `email` - the email of the new user
* `created_at` - the date and time the new user was created

#### GET /users

```bash
GET /users?id=123456789

Response:
{
  "id": 987654321,
  "name": "Jonathon Smith",
  "email": "jonathon.smith@smith.com",
  "created_at": "2022-01-24T12:34:56.000Z",
  "updated_at": "2022-01-25T09:12:34.000Z"
}
```
#### POST /users

```perl
POST /users
{
  "name": "Jane Doe",
  "email": "jane.doe@example.com",
  "password": "password123"
}

Response:
{
  "id": 987654321,
  "name": "Jane Doe",
  "email": "jane.doe@example.com",
  "created_at": "2022-01-25T10:00:00.000Z"
}
```
The Retrieve User Data API provides developers with a simple and straightforward way to retrieve user data from our system. We hope this API documentation has been helpful, and please feel free to contact us if you have any questions or concerns.
