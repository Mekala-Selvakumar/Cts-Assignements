# Assignment: Building a Demo Banking Application with Java/.NET/JS

**Objective:**
In this assignment, you will create a Java application to manage bank accounts. You will build a `Transaction` class with date, type, and amount, where the type is represented as an enum with 'debit' and 'credit'. The `Transaction` object should be created using the Builder pattern. You will also develop an abstract class, `Account`, that includes properties like account number, a list of transactions, balance, and opening date. You will then create two subclasses, `SBAccount` and `FDAccount`, each with its own properties and methods.

## Instructions:

### Transaction Class:
- Create a `Transaction` class with the following properties:
  - `date` as a object (ex. `LocalDate` in java)
  - `type` as an enum with 'debit' and 'credit'
  - `amount` as a double

- Implement a builder pattern to create `Transaction` objects.

### Abstract Account Class:
- Create an abstract class named `Account` with the following properties:
  - `accountNumber` (int)
  - `transactionList`, a list of `Transaction` objects
  - `balance` (double)
  - `openingDate` (LocalDate)

- Define the following methods:
  - `deposit`: Adds a credit transaction to the transaction list for each deposit.
  - `getAccountDetails`: Returns a string with the account details.

### SBAccount Class (Subclass of Account):
- Create an `SBAccount` class as a subclass of `Account` with the following additional properties:
  - `minBalance` (double)

- Implement the following method:
  - `withdraw`: Throws an `InsufficientBalanceException` if the amount is not available and adds a debit transaction to the transaction list for each withdrawal.

### FDAccount Class (Subclass of Account):
- Create an `FDAccount` class as a subclass of `Account` with the following additional properties:
  - `maturityDate` of type `LocalDate`
  - `interestRate` as a double

- Implement the following methods:
  - `getTenure`: Returns the tenure in months.
  - `getMaturityAmount`: Returns the maturity amount.



# Assignment: User Login Form with Validation

## Objective:
The objective of this case study is to create a user login form using HTML, CSS, and JavaScript. The form should have fields for username, password, and a remember me checkbox. The form should perform client-side validation, and the user's credentials should be matched with an existing users object in the code. Appropriate messages should be displayed on the same page.

## Instructions:

### HTML Form:

Create an HTML form that includes the following elements:
- Username input field
- Password input field (masked)
- Remember me checkbox
- Submit button

### CSS Styling:

- Style the form to make it visually appealing and user-friendly.
- Add CSS rules to provide visual feedback for successful and unsuccessful login attempts.

### JavaScript Functionality:

- Create a JavaScript function that will be triggered when the form is submitted.
- Implement client-side validation to check for the following:
  - Username is not empty.
  - Password is not empty.
  - Check if the "Remember Me" checkbox is checked.

### User Validation:

- Create an array or object in your JavaScript code containing predefined user credentials. For example:
```javascript
const users = [
  { username: "user1", password: "password1" },
  { username: "user2", password: "password2" },
  // Add more users if needed
];
```
# Matching Credentials

When the form is submitted and validation passes, check if the provided username and password match any user credentials in your predefined object.

# Display Messages

Display appropriate messages on the same page based on the following scenarios:

- Successful login (e.g., "Login successful! Welcome, [Username]").
- Invalid username or password (e.g., "Invalid credentials. Please try again.").
- If "Remember Me" is checked, display a message like "You will be remembered."

# Reset Form

Implement a button to reset the form for the user to try again after a failed login attempt.
