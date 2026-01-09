This project is an ASP.NET Core Web API developed in .NET 8 for managing a car fleet and their technical inspection details.  
The API is designed to be consumed by a mobile application (Xamarin /.NET MAUI).

The backend communicates with Microsoft SQL Server using **stored procedures (ADO.NET)**.

---

## Features
- Vehicle and technical inspection management
- RESTful APIs (GET, POST)
- SQL Server stored procedures for all database operations

---

## Technologies Used
- ASP.NET Core Web API (.NET 8)
- C#
- Microsoft SQL Server
- ADO.NET (SqlConnection, SqlCommand)
- Stored Procedures
- Dependency Injection

---

## Database Design
The SQL Server database contains:
- Vehicles table
- TechnicalTests table

All database operations are handled using stored procedures.

Database scripts are available in the `Database` folder.

---

## API Endpoints

### Vehicle APIs
- GET `/api/vehicles`  
  → Fetch vehicle and technical inspection details  
  → Supports filtering by registration number

- POST `/api/vehicles`  
  → Updates vehicle technical inspection data

---

## How to Run the Project
1. Clone the repository
2. Execute SQL scripts from the `Database` folder on local SQL Server
3. Update the connection string in `appsettings.json`
4. Run the project using Visual Studio or `dotnet run`
5. Test APIs using Postman or Swagger UI

---

## Notes
- Database access is implemented using stored procedures for better performance and security
