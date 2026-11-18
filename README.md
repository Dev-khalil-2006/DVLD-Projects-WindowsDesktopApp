Driving & Vehicle License Department (DVLD)
A desktop application developed using C# Windows Forms to manage driving-license department operations. The project uses a 3-Tier Architecture, ADO.NET, and Microsoft SQL Server to separate the user interface, business logic, and data-access responsibilities.
Overview
DVLD is designed to organize licensing-related records and workflows through a Windows desktop interface. It provides management features for people, drivers, applications, licenses, and tests while using a relational database to maintain structured data and reduce redundancy.
Technologies
- C#
- .NET Framework
- Windows Forms (WinForms)
- ADO.NET
- Microsoft SQL Server
- 3-Tier Architecture
- Stored Procedures
- Relational Database Design
Architecture
The application follows a 3-Tier Architecture:
┌──────────────────────────────┐
│     Presentation Layer      │
│       Windows Forms         │
└──────────────┬───────────────┘
               │
┌──────────────▼───────────────┐
│       Business Layer         │
│    Business Rules / Logic   │
└──────────────┬───────────────┘
               │
┌──────────────▼───────────────┐
│       Data Access Layer      │
│       ADO.NET / SQL          │
└──────────────┬───────────────┘
               │
┌──────────────▼───────────────┐
│      SQL Server Database     │
└──────────────────────────────┘
Layers
- Presentation Layer: Windows Forms screens and user interaction.
- Business Layer: Business rules, validation, and application operations.
- Data Access Layer: Database communication and data manipulation using ADO.NET and SQL Server.
This separation improves maintainability, organization, and the ability to modify a layer without tightly coupling the entire application.
Main Modules
- People Management — Manage people records and related information.
- Drivers Management — Manage driver records.
- Applications Management — Manage licensing applications and their information.
- Local Licenses — Handle local driving-license records and related operations.
- International Licenses — Handle international-license records.
- Tests Management — Manage tests associated with licensing workflows.
The modules and workflows available in the application depend on the implemented project version.

Database
The project uses a relational database in Microsoft SQL Server.

Database-related concepts and techniques used include:
- Relational database design
- Tables and relationships
- Data integrity
- CRUD operations
- ADO.NET for database connectivity and data manipulation
- Stored procedures
- Organized data management and reduced data redundancy
Key Concepts Demonstrated
- Applying 3-Tier Architecture in a desktop application
- Separating UI, business logic, and data access
- Object-oriented programming with C#
- Working with Windows Forms
- Connecting to and querying SQL Server using ADO.NET
- Implementing CRUD operations
- Using stored procedures
- Designing and working with relational databases
Getting Started
Prerequisites
- Windows
- Visual Studio with Windows Forms and .NET Framework development support
- Microsoft SQL Server
- SQL Server Management Studio (SSMS), recommended
Setup
1. Clone or download this repository.
2. Open the solution (.sln) in Visual Studio.
3. Create or restore the project's SQL Server database using the database files/scripts included in this repository (if provided).
4. Update the database connection string in the project configuration to match your SQL Server instance.
5. Build the solution.
6. Run the application.
Database setup steps and the exact connection-string location may vary based on the project configuration.

Screenshots
Add application screenshots here to demonstrate the main screens and workflows.
<!-- Example:
![DVLD Dashboard](Screenshots/dashboard.png)
-->Project Status
This project was developed as a practical C# application to apply software architecture, Windows Forms, database, and data-access concepts.
Author
Khalil Ali
