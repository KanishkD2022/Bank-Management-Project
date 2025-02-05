# Bank-Management-Project
Bank Management System

Introduction

The Bank Management System is a simple C-based project that allows users to manage bank accounts efficiently. This project provides functionalities such as creating new accounts, updating account details, making transactions, viewing customer lists, and deleting accounts. It operates using a file-based system (record.dat) to store and retrieve user information.
Features

Create New Account: Users can open a new bank account by providing personal details.

Update Account Information: Modify existing customer details such as address and phone number.

Transaction Handling: Deposit or withdraw money from an existing account.

Check Account Details: View information about an account using either account number or customer name.

Delete an Account: Remove an account from the records.

View Customer List: Display a list of all registered customers.

Secure Login System: Users must enter a password (codewithc) to access the system.

Installation and Usage

Prerequisites

A C compiler (GCC, MinGW, or Turbo C++)

Windows (for windows.h support) or a compatible OS

Compilation

To compile the project, use the following command:

gcc bank_management_project.c -o bank_management -Wall

Running the Program

Execute the compiled program:

./bank_management

Login

Upon execution, the system will prompt for a password. The default password is:

codewithc

After entering the correct password, the main menu will appear.

Project Structure

The project follows a modular approach, with the following key functions:

1. new_acc()

Adds a new account after verifying the uniqueness of the account number.

Stores user details in record.dat.

2. edit()

Allows modification of the address or phone number of an existing customer.

3. transact()

Enables users to deposit or withdraw money.

Prevents transactions for fixed deposit accounts.

4. see()

Displays account details using account number or name.

Calculates and displays interest for fixed and savings accounts.

5. erase()

Deletes a customer record permanently from record.dat.

6. view_list()

Displays all registered accounts along with essential details.

7. menu()

Provides an interactive menu for navigating through the system.

File Handling

The project uses record.dat to store all customer details.

Temporary files (new.dat) are used for updates and deletions.

The fscanf() and fprintf() functions handle reading and writing operations.

Security Considerations

The program includes a simple password mechanism for authentication.

Data is stored in a plain-text file (record.dat), which can be improved with encryption.
