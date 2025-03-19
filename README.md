Pharmacy Data Management System - "Farmacia Inimii"

Overview

"Farmacia Inimii" is a full-featured web-based system designed to manage data for pharmacies. The platform simplifies and centralizes operations such as inventory management, client tracking, supplier details, and production facilities. Built with scalability in mind, it can support both individual pharmacies and larger pharmacy networks.


Features

Secure User Authentication
Implements secure login with session management and hashed passwords, ensuring protection against unauthorized access.


Modular System Design

The system includes five core modules:
Medicines: Add, edit, delete, and view medicine records (name, production date, expiration date).
Pharmacies: Manage pharmacy branches (name, address, establishment date).
Producers: Register and maintain details about drug producers (name, country, headquarters).
Clients: Track client details and their interaction with pharmacies and medicines.
Factories: Link factories to producers and medicines for full production tracking.


Full CRUD Operations

Each module supports create, read, update, and delete functionalities with an intuitive web interface.


Data Validation

Front-end and back-end validation to ensure data integrity and prevent incomplete or invalid data entries.


Security Features

- Passwords hashed before storage.
- SQL injection prevention via prepared statements and input sanitization.
- Session-based access control.

  
Technologies Used

- Backend: PHP (modular structure with separate CRUD files)
- Database: MySQL (relational model with well-defined entity relationships)
- Frontend: HTML, CSS (responsive and user-friendly design)
- Security: PHP password hashing, parameterized SQL queries


Database Design

The relational database model includes the following associations:
- Clients are linked to pharmacies (1:N) and medicines (1:M)
- Factories are linked to medicines (1:N) and producers (1:M)
- A separate users table handles secure authentication (standalone)

  
How It Works

Login System:

Users authenticate using a secure form with session management.

Dashboard:

Once logged in, users can navigate between modules via a dashboard.

Data Management:
Users can add, edit, view, or delete records across all modules, with backend logic ensuring SQL injection prevention and proper data handling.

Admin Operations:
CRUD operations are handled via dedicated PHP scripts (e.g., medicamente.php, edit_medicament.php, etc.).

