# User Profile Management API

This is a RESTful API for managing user profiles with authentication.

## Features
- User Registration & Profile Creation
- User Profile Retrieval
- User Profile Update
- JWT Authentication
- Protected Routes (Users can access only their profiles)
- MongoDB Database Integration
- Error Handling

## Tech Stack
- **Backend:** Node.js, Express.js
- **Database:** MongoDB (Mongoose ODM)
- **Authentication:** JWT (JSON Web Token)

## Installation & Setup
### Prerequisites
- [Node.js](https://nodejs.org/) installed
- [MongoDB](https://www.mongodb.com/) installed or a MongoDB Atlas account

### Clone the Repository
```sh
git clone https://github.com/yourusername/user-profile-api.git
cd user-profile-api
```

### Install Dependencies
```sh
npm install
```

### Environment Variables
Create a `.env` file in the root directory and add:
```sh
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
```

### Start the Server
```sh
npm start
```

Server will run on `http://localhost:5000`

## API Endpoints
### User Authentication
#### Register a User
**POST** `/api/auth/register`
- Request Body:
```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "password": "123456"
}
```

#### Login a User
**POST** `/api/auth/login`
- Request Body:
```json
{
  "email": "john@example.com",
  "password": "123456"
}
```

### User Profile
#### Get Profile (Protected)
**GET** `/api/users/profile`
- Headers: `{ Authorization: Bearer <token> }`

#### Update Profile (Protected)
**PUT** `/api/users/profile`
- Headers: `{ Authorization: Bearer <token> }`
- Request Body:
```json
{
  "name": "John Updated",
  "bio": "New bio content",
  "profilePicture": "http://example.com/pic.jpg"
}
```

## Testing with Postman
1. Import the Postman Collection (link or JSON file)
2. Use the **Register** API to create a new user
3. Use the **Login** API to get a JWT token
4. Use the token in the **Authorization** header for protected routes

## Error Handling
- 400: Bad Request (Validation Errors)
- 401: Unauthorized (Invalid/Missing Token)
- 403: Forbidden (Access Denied)
- 404: Not Found

## Contribution
Feel free to fork, create a branch, and submit a PR.

## License
MIT

