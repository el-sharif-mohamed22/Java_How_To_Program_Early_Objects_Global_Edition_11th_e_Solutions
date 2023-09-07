# Chapter #3 Exercises

## 3.5 (Keyword new)

1. The purpose of the keyword `new` keyword is used to create an instance of a class.
2. What happens when you use it:

    - The `new` keyword instructs the JVM to allocate memory for the new object.
    - After memory allocation, the constructor of the class is invoked.
    - Then it returns a reference for the newly created object, this reference can be assigned to a variable, allowing access and manipulation of the objects's properties and methods.

## 3.6 (Default Constructors)

- You can't create an instance of the class with no parameters because once you declared a custom constructor (in this case the one that takes two parameters) then you can' use the default constructor (with no parameters), in order to do so you have to crate multiple constructors.

## 3.7 (Instance Variables)

- Instance variables are used to represents the attributes (properties) of a class, and its carried out with the class instances (objects), every instance maintain its own copy of this attributes.

## 3.8 (Using Classes without Importing Them)

- Because the `System` and `String` classes are part of the `java.lang` package which is imported by default in every java program, so you don't need to explicitly import them.

## 3.9 (set and get Methods)

- Without the use of setters the instance variable will be accessed directly from the driver class (if they aren't marked as `private`) which can modify the instance variable without validation and logic checks resulting invalid values.
- Without the use of setters and getters if you decide later to change the internal representation of an instance variable or add additional validation, then you may have to modify the entire code that directly accesses the variable.

## 3.10 (Modified account Class)

```java Account.java
// Account.java
public class Account {
    
    private String name;
    private double balance;

    public Account(String name, double balance) {
        this.name = name;
        if (balance > 0.0) {
            this.balance = balance;
        }
    }
    public void setName(String name) {
        this.name = name;
    }

    public String getName() {
        return name;
    }

    public void deposit(double depositAmount) {
        if (depositAmount > 0.0) {
            balance = balance + depositAmount;
        }
    }

    public void withdraw(double withdrawAmount) {
        if (withdrawAmount > balance) {
            System.out.println("Withdrawal amount exceeded account balance.");
        }
        if (withdrawAmount <= balance) {
            balance = balance - withdrawAmount;
        }
    }
    public double getBalance() {
        return balance;
    }

}
```

```java {id="AccountTest" class="blue large" data-filename="AccountTest.java"}
// AccountTest.java
// Inputting and outputting floating-point numbers with Account objects.
import java.util.Scanner;

public class AccountTest {
    public static void main(String[] args) {
        Account account1 = new Account("Jane Green", 50.00);
        Account account2 = new Account("John Blue", 90);

        // display initial balance of each object
        System.out.printf("%s balance: $%.2f%n",
                account1.getName(), account1.getBalance());
        System.out.printf("%s balance: $%.2f%n%n",
                account2.getName(), account2.getBalance());

        // create a Scanner to obtain input from the command window
        Scanner input = new Scanner(System.in);

        System.out.print("Enter withdraw amount for account1: "); // prompt
        double withdrawAmmount = input.nextDouble(); // obtain user input
        System.out.printf("%nwithdrawing %.2f to account1 balance%n%n", withdrawAmmount);
        account1.withdraw(withdrawAmmount); // remove from account1's balance

        // display balances
        System.out.printf("%s balance: $%.2f%n", account1.getName(), account1.getBalance());
        System.out.printf("%s balance: $%.2f%n%n", account2.getName(), account2.getBalance());

        System.out.print("Enter withdraw amount for account2: "); // prompt
        withdrawAmmount = input.nextDouble(); // obtain user input
        System.out.printf("%nwithdrawing %.2f to account2 balance%n%n", withdrawAmmount);
        account2.withdraw(withdrawAmmount); // add to account2 balance

        // display balances
        System.out.printf("%s balance: $%.2f%n", account1.getName(), account1.getBalance());
        System.out.printf("%s balance: $%.2f%n%n", account2.getName(), account2.getBalance());
    }
}
```