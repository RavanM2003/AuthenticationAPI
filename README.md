# Authentication API

This is an Authentication API built with .NET 8 and IdentityUser. This API provides endpoints for user registration, login, and user management.

## Features

- User Registration
- User Login
- User Management (CRUD operations)
- Secure Password Handling
- Token-Based Authentication

## Technologies Used

- .NET 8
- IdentityUser
- Entity Framework Core
- MSSQL

## Getting Started

### Installation

1. Clone the repository:

   ```sh
   git clone https://github.com/RavanM2003/AuthenticationAPI.git
   cd AuthenticationAPI
   ```

2. Update the connection string in `appsettings.json`:

   ```json
   {
     "ConnectionStrings": {
       "DefaultConnection": "YourConnectionStringHere"
     }
   }
   ```

3. Apply migrations and update the database:

   ```sh
   dotnet ef database update
   ```

4. Run the application locally:

   ```sh
   dotnet run
   ```

### Endpoints

#### Registration

- **URL**: `https://localhost:5001/register`
- **Method**: `POST`
- **Request Body**:

  ```json
  {
    "password": "string",
    "email": "string"
  }
  ```

#### Login

- **URL**: `https://localhost:5001/login`
- **Method**: `POST`
- **Request Body**:

  ```json
  {
    "username": "string",
    "password": "string",
    "twoFactorCode": "string",
    "twoFactorRecoveryCode": "string"
  }
  ```


## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License.
