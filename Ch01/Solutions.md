
# Self-Review Exercises Solutions

<p align="center">
  <h3 align="center">Chapter #1 Solutions</h3>
</p>

## Table of contents

- [1.1](#1_1)
- [1.2](#1_2)
- [1.3](#1_3)
- [1.4](#1_4)
- [1.5](#1_5)
- [1.6](#1_6)
- [1.7](#1_7)
- [1.8](#1_8)
- [1.9](#1_9)
- [1.10](#1_10)
- [1.11](#1_11)
- [1.12](#1_12)
- [1.13](#1_13)
- [1.14](#1_14)
- [1.15](#1_15)

## 1_1

1. a) Programs.
2. b) Input units, output units, ALU (arithmetic and logic unit), CPU (central processing unit), secondary storage unit, memory unit.
3. c) Machine Language, Assembly Language, High-Level Language.
4. d) Compilers.
5. e) Android.
6. f) Release Candidate.
7. g) accelerometer.

## 1_2

1. a) java "name of the file with .class extension".
2. b) javac "name of the file with .java extension".
3. c) .java.
4. d) .class.
5. e) Bytecode.

## 1_3

1. a) Information hiding.
2. b) Classes.
3. c) OOAD (object oriented analysis and design).
4. d) Inheritance.
5. e) UML (unified modeling language).
6. f) Attributes.

---

## 1_4

1. a) Input unit.
2. b) Programming.
3. c) Assembly.
4. d) Output devices.
5. e) Memory unit, secondary storage unit.
6. f) ALU (arithmetic and logical unit).
7. g) CPU (central processing unit).
8. h) High level languages.
9. i) Machine language.
10. j) CPU (central processing unit).

## 1_5

1. a) Java.
2. b) Java SE (standard edition), Java EE (enterprise edition), Java ME (micro edition).
3. c) Bandwidth.
4. d) Assembler.

## 1_6

1. a) Editing, compiling, loading, bytecode verification, and execution.
2. b) IDE (integrated development environment).
3. c) JVM (java virtual machine).
4. d) VM (virtual machine).
5. e) Class Loader.
6. f) Bytecode Validator.

## 1_7

JVM analyzes the bytecodes as they’re interpreted, searching for hot spots—bytecodes that execute frequently. For these parts, a just-in-time
(JIT) compiler, translates the bytecodes into the computer’s machine language. When the JVM encounters these compiled parts again, the faster machine-language code executes.

## 1_8

- Object: instances of wrist watches.
  - Omega wristwatch model 55 with serial 88.
  - Ahmad's Rolex wristwatch model 223 with serial 234.
- Attributes:
  - Size.
  - Color.
  - Weight.
  - Material.
  - Brand.
  - Angle of hour hand.
  - Angle of minute hand.
  - Angle of second hand.
- Behaviors:
  - Adjust date.
  - Adjust time.
  - Show time.
  - Show date.
- Class: A class of wrist watch contains the design, attributes and behaviors of the wrist watch.
- Inheritance: A new class of objects can be created conveniently by Inheritance the new class (called the subclass) starts with the characteristics of an existing class (called the superclass), possibly customizing them and adding unique characteristics of its own. In the wristwatch context an alarm clock may inherit from the wristwatch and adding new attributes (ringtone, alarm time) and new behaviors (setting alarm, snooze) and customizing inherited behaviors like adjusting date.
- Modeling: A wristwatch can be modeled by designing a class that represents its attributes and behaviors, allowing programmers to work with the concept in their code.
- Messages: Each message is implemented as a method call that tells a method of the object to perform its task, for example User sends a message to adjust the date to day (22).
- Encapsulation: The wristwatch class encapsulate the attributes and methods of the wrist watch.
- Interface: collections of related methods that typically enable you to
tell objects what to do, but not how to do it, basic interface may contains (adjust date, adjust time, show time, show date).
- Information Hiding:
  - The way of maintaining the time and date is hidden from the user.
  - The way of adjusting the time and date is hidden from the user.

## 1_9

```java
CO2 = Total_Amount * (CO2_Emission_Factor * Heating_Value) * Density
CH4 = ((Total_Amount * (CH4_Emission_Factor * Heating_Value) * Density) * GWP_CH4_Conversion)
N2O = ((Total_Amount * (N2O_Emission_Factor * Heating_Value) * Density) * GWP_N2O_Conversion)
```

## 1_10

The formula for BMI is weight in kilograms (kg) divided by height in meters squared (m2).

## 1_11


## 1_12

1. Read the whole paragraph word by word.
2. Have every gender-specific word with it's gender-neutral replacement.
3. When encountering a gender-specific word replace it with it's corresponding gender-neutral one.

This procudure might produce strange term like "woperchild" when it's replaceing a part of the word for example "Woman" have "man" in it so when replaced by person it becomes "Woperson" but person itself contains a son inside of it so when replaced it becomes "Woperchild".

## 1_13

It can help blind people by using voice assistants.

