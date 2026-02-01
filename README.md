# Bank
This is a simple Bank Management System implemented in C++. The application allows managing clients, performing transactions, and maintaining client data in a file-based storage system (Clients.txt). It provides a console-based interface for administrators to perform banking operations easily.

# 🏦 Bank Management Console Application

A **C++ Console-Based Bank Management System** for managing clients and performing banking transactions.  
This project demonstrates file-based data persistence, structured programming, and user-friendly console interfaces.

---

## 🚀 Features

### 1. Client Management
- **Add new clients** with unique account numbers.
- **Update client information** including name, phone, and balance.
- **Delete clients** with confirmation prompts.
- **Find a client** by account number.
- **List all clients** with detailed information and account balances.

### 2. Transactions
- **Deposit money** into client accounts.
- **Withdraw money** from client accounts (ensures balance validation).
- **View total balances** of all clients.

### 3. Data Storage
- All client data is stored in a **text file** (`Clients.txt`) using a custom delimiter (`#//#`).
- Supports **read, write, update, and delete operations** on the file.

### 4. Console Interface
- Clear and structured **Main Menu** and **Transactions Menu**.
- Displays data in **tables** for easy readability.
- Confirmation prompts for sensitive operations like deletion or transactions.

---

## 🛠️ Technical Details

- **Language:** C++  
- **File Handling:** `fstream` for persistent data storage.  
- **Data Structure:** `struct sClient` and `std::vector` for dynamic data management.  
- **Formatting:** `iomanip` for structured console output.  
- **Modular Design:** Functions for each feature for clarity and maintainability.

---

## 📂 File Structure

BankManagementApp.cpp // Main source code file.
Clients.txt // Stores client records in the format:.
// AccountNumber#//#PinCode#//#Name#//#Phone#//#AccountBalance


---

## 💻 How to Run

1. Ensure you have a **C++ compiler** (e.g., GCC, Visual Studio, Code::Blocks).  
2. Place `Clients.txt` in the same folder as the program (it will be created automatically if it doesn't exist).  
3. Compile the program:


🔹 Sample Operations

Adding a New Client:

Input account number, pin code, name, phone, and initial balance.

System prevents duplicate account numbers.

Deposit:

Enter account number and deposit amount.

System updates the balance immediately.

Withdraw:

Enter account number and withdrawal amount.

Validates that withdrawal does not exceed account balance.

Show Total Balances:

Displays all clients’ balances and the total sum of balances.

⚠️ Notes
All sensitive actions require user confirmation.

Numeric input is validated where necessary.

Designed for console-based usage, easy to navigate and maintain.



📌 Future Improvements
Add authentication for clients and admins.

Include transaction history logs for each client.

Improve user interface with color-coded outputs.

Implement data encryption for sensitive information.


```bash
g++ -o BankManagementApp BankManagementApp.cpp
Run the program:

./BankManagementApp
Use the Main Menu and Transactions Menu to navigate the application.
