# Exercise 1 : Control Structures

## Objective

This exercise demonstrates the use of PL/SQL control structures such as:

- IF statement
- FOR LOOP
- UPDATE statement
- DBMS_OUTPUT
- Conditional execution

---

## Scenario 1

Apply a 1% discount to loan interest rates for customers whose age is greater than 60 years.

### Logic

- Fetch all customers.
- Check whether Age > 60.
- Update the corresponding loan interest rate.
- Commit the transaction.

---

## Scenario 2

Promote customers to VIP status.

### Condition

Balance > 10000

### Logic

- Iterate through all customers.
- Check account balance.
- Set IsVIP = TRUE.

---

## Scenario 3

Send reminders for loans due within the next 30 days.

### Logic

- Fetch loans due within 30 days.
- Display reminder messages using DBMS_OUTPUT.

---

## PL/SQL Concepts Used

- Anonymous Block
- FOR LOOP
- IF Statement
- UPDATE
- COMMIT
- DBMS_OUTPUT.PUT_LINE

---

## Output

```
Loan interest rates updated successfully.

VIP customers updated successfully.

Reminder: Customer ID 101 has Loan ID 2001 due on 15-JUL-26
Reminder: Customer ID 102 has Loan ID 2003 due on 22-JUL-26
```

---

## Conclusion

This exercise demonstrates how PL/SQL control structures can automate business operations such as updating loan interest rates, promoting VIP customers, and generating loan reminders.