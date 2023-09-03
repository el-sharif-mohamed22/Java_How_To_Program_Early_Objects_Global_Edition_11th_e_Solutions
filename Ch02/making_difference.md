# Chapter #2 Making a Difference

## 2.33 (Body Mass Index Calculator)

```java
// Program that calculates the BMI, and the category.
import java.util.Scanner;

public class BodyMassIndex {
    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);

        System.out.print("Enter your weight in Kg: ");
        double weight = input.nextDouble();

        System.out.print("Enter your height in centimeters: ");
        double height = input.nextDouble();
        height = height / 100;
        double BMI = weight / (height * height);
        int category = 0;


        if (BMI >= 30) {
            category = 4;
        }
        if (BMI < 30) {
            category = 3;
        }
        if (BMI < 25) {
            category = 2;
        }
        if (BMI < 18.5) {
            category = 1;
        }

        System.out.printf("Your BMI = %f%n", BMI);

        if (category == 1) {
            System.out.println("You are underweight");
        }

        if (category == 2) {
            System.out.println("You have Normal weight");
        }

        if (category == 3) {
            System.out.println("You are Overweight");
        }

        if (category == 4) {
            System.out.println("You have Obesity");
        }
    }
}
```

## 2.34 (World Population Growth Calculator)

```java
// Program calculates the world population in 5 years.
import java.util.Scanner;
public class Population {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.print("Enter the current world population: ");
        long population = input.nextLong();

        System.out.print("Enter the annual world population growth rate: ");
        double growth = input.nextDouble();

        population = population + (long) (population * growth);
        System.out.printf("Expected world population after 1 year = %d%n", population);

        population = population + (long) (population * growth);
        System.out.printf("Expected world population after 2 year = %d%n", population);

        population = population + (long) (population * growth);
        System.out.printf("Expected world population after 3 year = %d%n", population);

        population = population + (long) (population * growth);
        System.out.printf("Expected world population after 4 year = %d%n", population);

        population = population + (long) (population * growth);
        System.out.printf("Expected world population after 5 year = %d%n", population);

    }
}

```