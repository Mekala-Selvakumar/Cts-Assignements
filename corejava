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
