 Simple Bank Account
1. Objective
To create a Python class that simulates a basic bank account, allowing a user to deposit money, withdraw money, and check balance while ensuring proper validations like insufficient balance checks.
2. Detailed Description
Students need to build a program that manages a customer’s bank account using a class named BankAccount. The class should store an account balance and provide functions to:
Deposit money: Add amount to the balance
Withdraw money: Subtract amount from the balance only if funds are sufficient
View balance: Show the current balance
The program must use a loop so the user can perform multiple transactions (deposit/withdraw/view balance) until they choose to exit.
There should also be a conditional check for insufficient balance. If a user tries to withdraw more than what they have, the program must display: “Insufficient Balance! Transaction cancelled.”
This simulates real-world banking operations and teaches students class structure, looping, and conditional logic.
3. Question Based on the Description
Write a Python program using a class BankAccount that:
Stores and manages an account balance.
Lets the user repeatedly choose to deposit, withdraw, or check balance using a loop.
Prevents withdrawal if balance is low and shows a proper message.
4. Conditional Question
Add a condition to your program:
If the user withdraws money and balance becomes less than ₹100, display a warning message: “Low Balance! Please maintain minimum ₹100.”

