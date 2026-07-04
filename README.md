# Students Management with Blazor

[![.NET](https://img.shields.io/badge/.NET-8.0-512BD4)](https://dotnet.microsoft.com/)
[![Blazor](https://img.shields.io/badge/Blazor-Web%20App-512BD4)](https://dotnet.microsoft.com/apps/aspnet/web-apps/blazor)

Students Management with Blazor is a modern web application for managing student-related records in an educational environment. Built with ASP.NET Core and Blazor, it provides a responsive and secure interface for handling students, parents, teachers, subjects, countries, and supporting reference data.

## Overview

This project demonstrates a full-stack Blazor application with a server-rendered experience and interactive client-side components. It combines a clean UI, data-driven workflows, and ASP.NET Core Identity for authentication, making it suitable as a foundation for school administration systems or similar CRUD-based business applications.

## Key Features

- Manage student records with personal, contact, and demographic details
- Maintain parent and teacher information with related metadata
- Organize academic subjects and associated descriptions
- Manage reference values such as countries and system codes
- Secure user authentication and account management with ASP.NET Core Identity
- Responsive UI powered by Blazor, Bootstrap, and AdminLTE styling
- Database-backed CRUD operations using Entity Framework Core

## Tech Stack

- ASP.NET Core 8
- Blazor Web App (Server + WebAssembly)
- Entity Framework Core
- SQL Server
- ASP.NET Core Identity
- Bootstrap / AdminLTE
- C# and Razor components

## Prerequisites

Before running the application, make sure you have the following installed:

- .NET 8 SDK
- SQL Server or SQL Server Express / LocalDB
- Visual Studio 2022 or VS Code
- Git

## Installation & Setup

1. Clone the repository

   ```bash
   git clone https://github.com/your-username/StudentsManagementWithBlazor.git
   cd StudentsManagementWithBlazor
   ```

2. Update the database connection string

   Open [StudentsManagement/appsettings.json](StudentsManagement/appsettings.json) and adjust the connection string to match your SQL Server instance.

3. Restore dependencies

   ```bash
   dotnet restore
   ```

4. Apply database migrations

   If the Entity Framework Core CLI is not installed yet, run:

   ```bash
   dotnet tool install --global dotnet-ef
   ```

   Then apply the migrations:

   ```bash
   dotnet ef database update --project StudentsManagement
   ```

5. Run the application

   ```bash
   dotnet run --project StudentsManagement
   ```

6. Open your browser and navigate to:

   ```text
   https://localhost:7226
   ```

## Usage Examples

Once the application is running, you can:

- Register a new user account or sign in
- Create and manage student profiles
- Add parent and teacher records
- Maintain subject and reference data through the administrative interface

Example startup commands:

```bash
dotnet restore
dotnet build
dotnet run --project StudentsManagement
```

## Contributing

Contributions are welcome. To contribute:

1. Fork the repository
2. Create a feature branch
3. Implement your changes and keep the code clean
4. Submit a pull request with a clear description of the improvement

Please make sure your changes are well-documented and aligned with the project’s existing architecture.

## License

This project currently does not include a license file. If you plan to publish or share it publicly, consider adding an open-source license such as MIT.
