# ATM Core Java Project

A simple **ATM console-based mini project** built using **Core Java**.  
This project simulates basic ATM operations such as login, account selection, balance checking, withdrawal, and deposit.

## Features

- Customer login using **customer number** and **PIN**
- Access **Checking Account** and **Savings Account**
- View account balance
- Withdraw money
- Deposit money
- Console-based menu navigation
- Currency formatting in **Indian Rupees (₹)**

## Project Structure

```text
ATM.java
Account.java
OptionMenu.java
```

### 1. `ATM.java`
- Contains the `main()` method
- Starts the application
- Calls the login menu

### 2. `Account.java`
- Stores account-related data:
  - customer number
  - PIN number
  - checking balance
  - saving balance
- Contains methods for:
  - balance retrieval
  - deposit calculation
  - withdrawal calculation
  - user input for deposit/withdraw operations

### 3. `OptionMenu.java`
- Extends `Account`
- Handles:
  - login validation
  - account type selection
  - checking and saving account menus
- Uses `HashMap` to store sample customer numbers and PINs

## Technologies Used

- Core Java
- OOP concepts
- Inheritance
- HashMap
- Scanner
- DecimalFormat

## Sample Login Credentials

The project currently uses hardcoded login data:

- Customer Number: `942486547`  
  PIN: `9171`

- Customer Number: `810754451`  
  PIN: `9893`

## How to Run

1. Open the project in any Java IDE such as:
   - IntelliJ IDEA
   - Eclipse
   - VS Code

2. Make sure all files are inside the same package:

```java
package zProject1;
```

3. Compile and run `ATM.java`

## Example Flow

1. User enters customer number
2. User enters PIN
3. User selects account type:
   - Checking
   - Savings
4. User chooses an operation:
   - View Balance
   - Withdraw Funds
   - Deposit Funds
   - Exit

## Code Highlights

- `ATM.java` starts the program and calls `getLogin()` to begin the ATM flow.
- `OptionMenu.java` manages login and user menu navigation.
- `Account.java` handles balance operations for checking and savings accounts.

## Notes

- This is a **beginner-friendly Core Java project**
- It is designed for learning:
  - classes and objects
  - inheritance
  - user input handling
  - menu-driven programs

## Current Limitations

- Login data is hardcoded
- No database connection
- No file handling
- No transaction history
- Balances reset when the program restarts

## Important Improvement Suggestions

There are a couple of logic issues in the current code that can be improved:

- In deposit methods, withdrawal methods are being called instead of deposit methods
- Some menu text and account labels can be cleaned up
- Input validation can be made stronger
- Wrong login message may still print even after a correct login flow

## Future Enhancements

- Add database integration
- Add transaction history
- Add PIN change feature
- Add money transfer feature
- Add proper exception handling
- Improve menu design

## Author

ATM Mini Project in Core Java for practice and learning.
