class BankAccount:
    def __init__(self, balance=0):
        self.balance = balance

    def deposit(self, amount):
        if amount > 0:
            self.balance += amount
            print(f"₹{amount} deposited successfully.")
        else:
            print("Invalid amount! Deposit must be greater than 0.")

    def withdraw(self, amount):
        if amount <= 0:
            print("Invalid amount! Enter a positive value.")
        elif amount > self.balance:
            print("Insufficient Balance! Transaction cancelled.")
        else:
            self.balance -= amount
            print(f"₹{amount} withdrawn successfully.")

            # Low balance warning
            if self.balance < 100:
                print("Low Balance! Please maintain minimum ₹100.")

    def show_balance(self):
        print(f"Current Balance: ₹{self.balance}")


# ------ Main Program -------
account = BankAccount()

while True:
    print("\n----- Bank Menu -----")
    print("1. Deposit")
    print("2. Withdraw")
    print("3. View Balance")
    print("4. Exit")

    choice = input("Enter your choice (1-4): ")

    if choice == "1":
        amount = float(input("Enter amount to deposit: "))
        account.deposit(amount)

    elif choice == "2":
        amount = float(input("Enter amount to withdraw: "))
        account.withdraw(amount)

    elif choice == "3":
        account.show_balance()

    elif choice == "4":
        print("Thank you for using the bank system!")
        break

    else:
        print("Invalid choice! Please select again.")
