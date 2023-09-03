# Chapter #2 Exercises

## 2.7 Fill in the blanks in each of the following statements

1. a) comments.
2. b) `if` statement.
3. c) division `/` and reminder `%`.
4. d) innermost.
5. e) variable.

## 2.8 Write Java statements that accomplish each of the following tasks

1. a)

    ```java
    System.out.print("Enter an integer: ");
    ```

2. b)

    ```java
    int a = b * c;
    ```

3. c)

    ```java
    // Program that performs a sample payroll calculation.
    ```

## 2.9 State whether each of the following is true or false. If false, explain why

1. a) `True`, because parenthesis have a higher precedence.
2. b) `False`, because `X!` has the character `!`, and `a@b` has the character `@`. and a valid identifier consists of upper and lower case letters, numbers, underscores and dollar sign.
3. c) `False`, division has a higher precedence so `5 / 4` will be evaluated first.
4. d) `True`.

## 2.10 What does each of the following statements display

1. a)

    ```bat
    x = 10

    ```

2. b)

    ```bat
    Value of 5 *1 is 5
    
    ```

3. c)

    ```bat
    x is 5 and y is 1
    ```

4. d)

    ```bat
    6 is not equal to 5

    ```

## 2.11 Which of the following Java statements contain variables whose values are not modified

* a) variable p's value isn't modified.
* c) variable p's value isn't modified.
* d) variable k's value isn't modified.

## 2.12 which of the following are correct Java statements for this equation

* a) `y = a * x * x + 5 * x + 2;`
* b) `y = a * x * x + (5 * x) + 2;`
* d) `y = a * (x * x) + 5 * x + 2;`

## 2.13 What is the output that will be printed after execution of the following Java code snippet

```bat
1314
```

```mermaid
---
title: First statement results to 13
---
flowchart TB
    +-->p
    +-->*
    *-->2
    *-->4 
```

```mermaid
---
title: Second statement results to 14
---
flowchart TB
    *-->p
    *-->2
    +-->*
    +-->4 
```

## 2.14 Write an application

1. a)

    ```java
    System.out.println("1 2 3 4");
    ```

2. b)

    ```java
    System.out.print("1 2 3 4\n");
    ```

3. c)

    ```java
    System.out.printf("%d %d %d %d%n", 1, 2, 3, 4);
    ```

## 2.15 (Arithmetic) Write an application

```java
// program that takes two integers then make some calculations.

import java.util.Scanner;

public class Arithmetic {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Enter first integer: ");
        int number1 = input.nextInt();

        System.out.print("Enter second integer: ");
        int number2 = input.nextInt();

        int num1Squared = number1 * number1;
        int num2Squared = number2 * number2;

        System.out.printf("Square of first integer = %d%n", num1Squared);
        System.out.printf("Square of second integer = %d%n", num2Squared);
        System.out.printf("The sum of the squares = %d%n", num1Squared + num2Squared);
        System.out.printf("The difference of the squares = %d%n", num1Squared - num2Squared);
        
    }
}
```

## 2.16 (Comparing Integers) Write an application

```java
// Program that takes an integer and make some comparisons on the number and its square.

import java.util.Scanner;

public class Compare {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Enter an integer: ");
        int num = input.nextInt();
        int square = num * num;

        // case 1: check if the number and its square are greater than 100.
        if (num > 100) {
            // if the num > 100 then for sure (num * num) > 100
            System.out.println("The number and its square are greater than 100.");
        }

        // case 2: check if the number and its square are equal to 100.
        // this case will never happen because if num = 100, then 100 * 100 != 100

        // case 3: check if the number and its square are not equal to 100.
        if (num != 100) {
            if (square != 100) {
                System.out.println("The number and its square are not equal to 100.");
            }
        }

        // case 4: check if the number and its square are less than 100.
        if (num < 100) {
            if (square < 100) {
                System.out.println("The number and its square are less than 100.");
            }
        }
    }
}
```

## 2.17 (Arithmetic, Smallest and Largest) Write an application

```java
// Program that takes three integers, calculate sum, average, smallest and largest.

import java.util.Scanner;

public class Arithmetic {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Enter the first number: ");
        int num1 = input.nextInt();

        System.out.print("Enter the second number: ");
        int num2 = input.nextInt();

        System.out.print("Enter the third number: ");
        int num3 = input.nextInt();

        int sum = num1 + num2 + num3;
        int average = sum / 3;
        
        // if there are a number less than the smallest then smallest takes that number.        
        int smallest = num1;
        if (smallest > num2) {
            smallest = num2;
        }
        if (smallest > num3) {
            smallest = num3;
        }

        // if there are a number greater than the largest then largest takes that number.
        int largest = num1;
        if (largest < num2) {
            largest = num2;
        }
        if (largest < num3) {
            largest = num3;
        }

        System.out.printf("Sum of the three number = %d%n", sum);
        System.out.printf("Average of the three number = %d%n", average);
        System.out.printf("Smallest of the three number = %d%n", smallest);
        System.out.printf("largest of the three number = %d%n", largest);
        
    }
}

```

## 2.18 (Displaying Shapes with Asterisks) Write an application

```java
// Program that displays a box, an oval, an arrow and a diamond using asterisks.

public class Shapes {
    public static void main(String[] args) {

        System.out.println("*********     ***       *        *");
        System.out.println("*       *   *     *    ***      * *");
        System.out.println("*       *  *       *  *****    *   *");
        System.out.println("*       *  *       *    *     *     *");
        System.out.println("*       *  *       *    *    *       *");
        System.out.println("*       *  *       *    *     *     *");
        System.out.println("*       *  *       *    *      *   *");
        System.out.println("*       *   *     *     *       * *");
        System.out.println("*********     ***       *        *");
    }

}

```

## 2.19 What does the following code print

```bat
  ****
 ******
*******
 ******
  ****

```

## 2.20 What does the following code print

```bat
*
***
*****
****
**

```

## 2.21 What does the following code print

```bat
***************

```

## 2.22 What does the following code print

```bat
****
*****
******

```

## 2.23 What does the following code print

```bat
  *
 *** 
*****
 ***
  *

```

## 2.24 (Largest and Smallest Integers) Write an application

```java
// Program that determines the largest and smallest among 5 integers

import java.util.Scanner;
public class Finder {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        
    }
}```