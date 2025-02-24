# Java Control Flow Statements: If and Switch

## Table of Contents
1. [Introduction](#introduction)
2. [If Statement](#if-statement)
   - [Syntax](#syntax)
   - [Examples](#examples)
3. [Switch Statement](#switch-statement)
   - [Syntax](#syntax)
   - [Examples](#examples)
4. [Conclusion](#conclusion)

## Introduction
Control flow statements in Java allow you to dictate the order in which statements are executed. Two fundamental control flow statements are `if` and `switch`. These statements enable you to make decisions in your code based on certain conditions.

## If Statement

The `if` statement is used to evaluate a boolean expression and execute a block of code if the expression is true. It can be extended with `else` and `else if` to handle multiple conditions.

### Syntax
```java
if (condition) {
    // Code to execute if condition is true
} else if (anotherCondition) {
    // Code to execute if anotherCondition is true
} else {
    // Code to execute if none of the conditions are true
}
```

### Examples

**Example 1: Basic If Statement**
```java
int number = 10;
if (number > 5) {
    System.out.println("Number is greater than 5");
}
```

**Example 2: If-Else Statement**
```java
int number = 3;
if (number > 5) {
    System.out.println("Number is greater than 5");
} else {
    System.out.println("Number is not greater than 5");
}
```

**Example 3: If-Else If-Else Statement**
```java
int number = 7;
if (number > 10) {
    System.out.println("Number is greater than 10");
} else if (number > 5) {
    System.out.println("Number is greater than 5 but less than or equal to 10");
} else {
    System.out.println("Number is 5 or less");
}
```

## Switch Statement

The `switch` statement allows you to execute one block of code out of many based on the value of a variable. It's a more readable alternative to multiple `if-else-if` statements when dealing with a single variable that can take multiple values.

### Syntax
```java
switch (variable) {
    case value1:
        // Code to execute if variable equals value1
        break;
    case value2:
        // Code to execute if variable equals value2
        break;
    // You can have any number of case statements
    default:
        // Code to execute if variable doesn't match any case
        break;
}
```

### Examples

**Example 1: Basic Switch Statement**
```java
int day = 3;
switch (day) {
    case 1:
        System.out.println("Monday");
        break;
    case 2:
        System.out.println("Tuesday");
        break;
    case 3:
        System.out.println("Wednesday");
        break;
    case 4:
        System.out.println("Thursday");
        break;
    case 5:
        System.out.println("Friday");
        break;
    case 6:
        System.out.println("Saturday");
        break;
    case 7:
        System.out.println("Sunday");
        break;
    default:
        System.out.println("Invalid day");
        break;
}
```

**Example 2: Switch Statement with String**
```java
String fruit = "Apple";
switch (fruit) {
    case "Apple":
        System.out.println("It is an apple");
        break;
    case "Banana":
        System.out.println("It is a banana");
        break;
    case "Orange":
        System.out.println("It is an orange");
        break;
    default:
        System.out.println("Unknown fruit");
        break;
}
```

## Conclusion
The `if` and `switch` statements are essential tools for controlling the flow of your Java programs based on conditions. Use `if` for complex conditions and boolean expressions, and `switch` for simpler, single-variable conditions with multiple possible values. Both statements enhance the readability and maintainability of your code.