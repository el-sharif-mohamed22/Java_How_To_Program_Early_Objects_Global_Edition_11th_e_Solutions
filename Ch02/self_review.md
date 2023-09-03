# Chapter #2 Self-Review Exercises

## Table of contents

- [2.1](#fill-in-the-blanks)
- [2.2](#state-whether-true-or-false)
- [2.3](#write-statements-to-accomplish-each-of-the-following-tasks)
- [2.4](#identify-and-correct-the-errors)
- [2.5](#write-declarations-statements-or-comments)
- [2.6](#write-a-complete-program)

## Fill in the blanks

2. a) left curly brace `{`, and right curly brace `}`.
2. b) if statements.
3. c) double forward slashes `//`.
4. d) spaces, tabs and end-lines.
5. e) keywords.
6. f) main method `public static void main(String[] args)`.
7. g)

    ```java
        System.out.println();
        System.out.print(); 
        System.out.printf();
    ```

## State whether true or false

1. a) `FALSE`, comments are ignored by the compiler.
2. b) `TRUE`.
3. c) `FALSE`, java is a case sensitive language so number and NumMbEr are considered to be different.
4. d) `FALSE`, can be used with other types like `long`.
5. e) `FALSE`, `*`, `/` and `%` have a higher precedence than `+` and `-`.
6. f) `FALSE`, starting from java 9 `_` (underscore) is no longer a valid identifier.

## Write statements to accomplish each of the following tasks

1. a)

    ```java
    int c = 0;
    int thisIsAVariable = 0;
    int q76454 = 0;
    ```

2. b)

    ```java
    System.out.print("Enter a number: ");
    ```

3. c)

    ```java
    int value = input.nextInt();
    ```

4. d)

    ```java
    System.out.println("This is a Java program");
    ```

5. e)

    ```java
    System.out.printf("%s%n%s", "This is a Java", " program");
    ```

6. f)

    ```java
    if (number != 7) {
        System.out.printf("%s%n", "The variable number is not equal to 7");
    }
    ```

## Identify and correct the errors

1. a) logical error a semicolon follows the if statement which will always execute the body of the if statement wether the condition is met or not. fix:

    ```java
    if (c < 7) {
        System.out.println("c is less than 7");
    }
    ```

2. b) compiler error the relational operator greater than or equal is written as `>=` not `=>`. fix:

    ```java
    if (c <= 7) {
        System.out.println("c is equal to or greater than 7");
    }
    ```

## Write declarations, statements or comments

1. a)

    ```java
    // program that calculates the product of three integers.
    ```

2. b)

    ```java
    // assume java.util.Scanner is imported.
    Scanner input = new Scanner(System.in);
    ```

3. c)

    ```java
    System.out.print("Enter first integer: ");
    ```

4. d)

    ```java
    int x = input.nextInt();
    ```

5. e)

    ```java
    System.out.print("Enter second integer: ");
    ```

6. f)

    ```java
    int y = input.nextInt();
    ```

7. g)

    ```java
    System.out.print("Enter third integer: ");
    ```

8. h)

    ```java
    int z = input.nextInt();
    ```

9. i)

    ```java
    int result = x * y * z;
    ```

10. j)

    ```java
    System.out.printf("Product is %d", result);
    ```

## write a complete program

```java
// program that calculates the product of three integers.

import java.util.Scanner;

public class Product{
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.print("Enter first integer: ");
        int x = input.nextInt();
        System.out.print("Enter second integer: ");
        int y = input.nextInt();
        System.out.print("Enter third integer: ");
        int z = input.nextInt();
        int result = x * y * z;
        System.out.printf("Product is %d%n", result);
    }
}
```
