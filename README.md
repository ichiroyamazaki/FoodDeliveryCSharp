# FoodDeliveryCSharp

FoodDeliveryCSharp is a C# Windows Forms application designed as a Food Delivery Point of Sale (POS) system. It uses a graphical interface and SQL Server LocalDB for account-related database operations.

## Overview

The project demonstrates a desktop application for food delivery operations. It includes account registration and login screens and uses a database to validate administrator credentials.

## Features

- **Login System:** Checks administrator credentials against the database.
- **Account Registration:** Allows users to register administrator accounts.
- **Password Visibility:** Provides a control to show or hide password input.
- **Input Validation:** Checks for empty login and registration fields.
- **Database Integration:** Uses SQL Server LocalDB through ADO.NET.
- **Windows Forms Interface:** Provides a graphical desktop application.
- **Multiple Forms:** Separates application screens into different Windows Forms.

The repository contains several form classes. Review the source code to confirm the full extent of its food ordering, menu, payment, and POS functionality.

## Requirements

- Windows operating system
- Visual Studio with Windows Forms support
- Compatible .NET Framework development tools
- SQL Server LocalDB
- The project source files

## Installation

1. Install Visual Studio with the required C# and Windows desktop development components.
2. Ensure SQL Server LocalDB is installed.
3. Clone or download the repository:

   ```bash
   git clone https://github.com/ichiroyamazaki/FoodDeliveryCSharp.git
   ```

4. Open the project in Visual Studio if a solution or project file is available.
5. Configure the database connection string in the source code.
6. Ensure the required database file and tables exist.
7. Build and run the application.

## Database Configuration

The source code uses SQL Server LocalDB and references a database file named `Koshigaya.mdf`.

The current connection string contains a machine-specific file path. Update it to point to the database file's actual location on your computer.

The login and registration code uses an `admin` table with fields for usernames, passwords, and account creation dates. The database schema must match the queries in the application.

**Security note:** The current source code stores and compares passwords directly. This is not recommended for production software. Use secure password hashing and parameterized SQL queries for all database operations.

## Project Structure

The repository includes these C# form files:

- `Form1.cs` - Login form
- `Form2.cs` - Registration form
- `Form3.cs` - Additional application screen
- `Form4.cs` - Additional application screen
- `Form9.cs` - Additional application screen
- `README.md` - Project documentation

## Project Information

| Detail | Description |
|---|---|
| Project Name | FoodDeliveryCSharp |
| Language | C# |
| UI Framework | Windows Forms |
| Database | SQL Server LocalDB |
| Application Type | Food Delivery POS |
| Developer | Ichiro Yamazaki |

## Disclaimer

This project is intended for educational and demonstration purposes. Review the database configuration and security practices before using it with real customer or business information.

## License

No license has been specified in this README. Refer to the repository for any license included with the source code.
