# Bank Management System

## Overview
The Bank Management System is a secure and robust application designed to manage users' financial activities efficiently. The system leverages Object-Oriented Programming (OOP) principles and Object-Oriented Design (OOD) patterns to ensure maintainability, scalability, and adherence to industry standards. Permissions and access control are implemented using a binary system within a Data Structures and Algorithms (DSA) framework, providing fine-grained role management.

## Features
1. **User Authentication:**
   - Secure login and logout functionality for all users.
   - Password hashing and validation mechanisms.

2. **Role-Based Permissions:**
   - Role differentiation: Admin and Regular User.
   - Permissions are managed using a binary representation system, ensuring efficient role verification and updates.

3. **Account Transactions:**
   - Transfer funds between user accounts.
   - Track transaction history.
   - Validate transactions to prevent fraud.

4. **Admin Features:**
   - Create, update, and delete user accounts.
   - Assign or modify user roles (Admin or Regular User).
   - View comprehensive system logs.

5. **Scalability and Performance:**
   - Optimized algorithms for transaction processing.
   - Modular design for future feature additions.

---

## System Design

### Class Structure

1. **User Class:**
   - Attributes: `UserID`, `Username`, `Password`, `Role`, `AccountBalance`.
   - Methods:
     - `Login()`
     - `Logout()`
     - `ViewAccountDetails()`

2. **Admin Class (Inherits from User):**
   - Methods:
     - `CreateUser()`
     - `DeleteUser()`
     - `ModifyPermissions()`
     - `ViewLogs()`

3. **Transaction Class:**
   - Attributes: `TransactionID`, `SenderID`, `ReceiverID`, `Amount`, `Timestamp`.
   - Methods:
     - `InitiateTransaction()`
     - `ValidateTransaction()`
     - `SaveTransaction()`

4. **PermissionsManager Class:**
   - Utilizes a binary system for role management.
   - Methods:
     - `AssignRole()`
     - `CheckPermissions()`

### Data Structures
- **Binary System for Permissions:**
  - Admin: `1111` (Full Access)
  - Regular User: `0011` (Limited Access)

- **Data Storage:**
  - Users: Stored in a map with `UserID` as the key.
  - Transactions: Stored in a list for chronological tracking.

---

## How to Use

### Setting Up
1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Compile the code using any C++ compiler.
   ```bash
   g++ -o BankSystem main.cpp
   ```
3. Run the executable:
   ```bash
   ./BankSystem
   ```

### User Workflow
1. **Login:**
   - Enter valid credentials to access the system.
2. **Perform Actions:**
   - Admins can manage users and view logs.
   - Users can view their account details and transfer funds.
3. **Logout:**
   - Ensure secure logout to terminate the session.

---

## Example Scenarios

1. **Admin Creating a User:**
   - Admin logs in and uses `CreateUser()` to add a new account.
   - Assigns a role to the user using `AssignRole()`.

2. **User Transferring Funds:**
   - User logs in and initiates a transaction with `InitiateTransaction()`.
   - The system validates the transaction and updates balances.

3. **Checking Permissions:**
   - A binary check ensures users have access to requested actions.

---

## Technologies Used
- **Programming Language:** C++
- **Design Principles:** OOP, OOD
- **Algorithms:** Binary search, Hashing
- **Data Structures:** Maps, Lists, Binary Trees

---

## Future Enhancements
1. Integrate a database for persistent data storage.
2. Add support for multiple currencies.
3. Implement a web-based interface using APIs.
4. Enhance security with multi-factor authentication (MFA).

---

## Contributors
- **Developer:** [Your Name]

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.
