# Bank System Project

## Overview
The Bank System is a robust, object-oriented project developed in C++ utilizing Object-Oriented Design (OOD) principles. It features functionalities for user authentication, role-based permissions, and account transfers, all built with a focus on scalability and security. The permission system is implemented using binary system data structures and algorithms (DSA).

---

## Features

### 1. User Authentication
- **Login**: Secure user authentication with username and password.
- **Logout**: Ensures active sessions are terminated securely.

### 2. Role-Based Permissions
- **Admin Role**: 
  - Manage users (add, update, delete accounts).
  - View all transactions.
  - Generate system reports.
- **Standard User Role**:
  - View account details.
  - Perform balance inquiries.
  - Transfer funds to other accounts.

### 3. Account Transfers
- Secure fund transfers between accounts.
- Logs and tracks each transaction for transparency.

### 4. Permission Management
- Built using binary system data structures.
- Flexible system to assign and manage roles dynamically.

---

## Implementation Details

### Object-Oriented Design Principles
The project adheres to the following principles:
- **Single Responsibility Principle (SRP)**: Each class has a single, well-defined responsibility.
- **Open/Closed Principle (OCP)**: Classes are open for extension but closed for modification.
- **Liskov Substitution Principle (LSP)**: Ensures derived classes can substitute their base classes without altering functionality.
- **Interface Segregation Principle (ISP)**: Interfaces are client-specific to avoid unnecessary dependencies.
- **Dependency Inversion Principle (DIP)**: High-level modules are not dependent on low-level modules; both rely on abstractions.

### Technology Stack
- **Programming Language**: C++
- **Data Structures**: Binary system for permission management.

---

## File Structure
```
BankSystem/
├── src/
│   ├── main.cpp              # Entry point of the application.
│   ├── User.cpp              # Handles user-related operations.
│   ├── Admin.cpp             # Handles admin-specific operations.
│   ├── Account.cpp           # Manages account details and transactions.
│   └── PermissionManager.cpp # Binary system for role-based permissions.
├── include/
│   ├── User.h                # Header file for User class.
│   ├── Admin.h               # Header file for Admin class.
│   ├── Account.h             # Header file for Account class.
│   └── PermissionManager.h   # Header file for PermissionManager class.
├── docs/
│   └── README.md             # Project documentation.
└── build/
    └── (compiled binaries)
```

---

## Getting Started

### Prerequisites
- C++ Compiler (e.g., GCC, Clang, or Visual Studio Compiler)
- CMake (optional, for build automation)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/bank-system.git
   ```
2. Navigate to the project directory:
   ```bash
   cd bank-system
   ```
3. Compile the project:
   ```bash
   g++ -o BankSystem src/*.cpp
   ```

4. Run the executable:
   ```bash
   ./BankSystem
   ```

---

## Usage

### Admin Workflow
1. Login as Admin.
2. Manage user accounts (add/update/delete).
3. View all transactions and generate system reports.

### User Workflow
1. Login with valid credentials.
2. View account balance.
3. Transfer funds securely to other accounts.

---

## Future Enhancements
- **Encryption**: Enhance security by encrypting sensitive data.
- **Database Integration**: Replace file-based storage with an SQL/NoSQL database.
- **Mobile App Support**: Extend functionality to mobile platforms.

---

## Contribution
Contributions are welcome! Please fork the repository and create a pull request with detailed descriptions of your changes.

---

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Contact
For any inquiries or feedback, please reach out to:
- **Name**: Zeyad
- **Email**: zeyad@example.com
