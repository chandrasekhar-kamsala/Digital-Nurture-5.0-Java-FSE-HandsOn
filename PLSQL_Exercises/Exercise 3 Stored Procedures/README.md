# Exercise 3 : Stored Procedures

## Objective

This exercise demonstrates how to create and execute stored procedures in PL/SQL.

---

## Scenario 1

### ProcessMonthlyInterest

Applies 1% monthly interest to all Savings accounts.

### Logic

- Select Savings accounts
- Increase balance by 1%
- Commit changes

---

## Scenario 2

### UpdateEmployeeBonus

Updates employee salaries by adding a bonus percentage.

### Parameters

- Department
- Bonus Percentage

---

## Scenario 3

### TransferFunds

Transfers money from one account to another.

### Validation

- Check sender balance
- If sufficient:
  - Deduct amount
  - Credit receiver
- Otherwise display an error message

---

## PL/SQL Concepts Used

- Stored Procedures
- Parameters
- Variables
- IF Statement
- UPDATE
- SELECT INTO
- COMMIT
- DBMS_OUTPUT

---

## Sample Output

```
Monthly interest processed successfully.

Employee bonus updated successfully.

Transfer Successful.
```

---

## Conclusion

Stored procedures improve code reusability, maintainability, and database performance by encapsulating business logic within the database.