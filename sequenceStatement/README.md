
# Sequence Statements, Variables, and Operators in Java

### Introduction
In Java, the sequence of execution is a fundamental concept. The program flows from top to bottom, executing statements in the order they are written. This README focuses on sequence statements, the use of variables, and operators in Java programs.

---

### 1. **Sequence of Execution in Java**

In a Java program, the sequence is how the statements are executed, one after another. Each statement has a specific order and is executed sequentially unless control flow statements (like `if`, `while`, `for`, etc.) alter the order.

#### 1.1 **Basic Sequence Example**
Consider the following program:

```java
public class SequenceExample {
    public static void main(String[] args) {
        int number = 10; // First statement
        number = number + 5; // Second statement
        System.out.println("The result is: " + number); // Third statement
    }
}
```

**Output:**
```
The result is: 15
```

In this example:
1. `int number = 10;` declares and initializes the variable.
2. `number = number + 5;` updates the value of `number`.
3. `System.out.println("The result is: " + number);` prints the updated value.

The execution follows the sequence from top to bottom, line by line.

---

### 2. **Variables in Java**

Variables are used to store data that can be referenced and manipulated throughout a program. In Java, you need to declare a variable before using it.

#### 2.1 **Variable Declaration**

To declare a variable, specify the data type followed by the variable name.

```java
int age; // Declare an integer variable 'age'
String name; // Declare a string variable 'name'
```

#### 2.2 **Variable Initialization**

Variables need to be initialized with a value before they can be used.

```java
age = 25; // Initialize 'age' with value 25
name = "John"; // Initialize 'name' with value "John"
```

#### 2.3 **Example: Using Variables**

```java
public class VariableExample {
    public static void main(String[] args) {
        int number = 10;
        String greeting = "Hello, World!";
        System.out.println(greeting + " The number is: " + number);
    }
}
```

**Output:**
```
Hello, World! The number is: 10
```

In this example:
- `number` is an integer variable.
- `greeting` is a string variable.

---

### 3. **Operators in Java**

Operators are symbols used to perform operations on variables and values. In Java, there are several types of operators, including arithmetic, assignment, comparison, and logical operators.

#### 3.1 **Arithmetic Operators**

These operators are used to perform mathematical operations.

- `+` (Addition)
- `-` (Subtraction)
- `*` (Multiplication)
- `/` (Division)
- `%` (Modulus)

Example:
```java
int x = 10;
int y = 5;
int sum = x + y; // Addition
int diff = x - y; // Subtraction
int product = x * y; // Multiplication
int quotient = x / y; // Division
int remainder = x % y; // Modulus
```

#### 3.2 **Assignment Operators**

These operators are used to assign values to variables.

- `=` (Assigns value)
- `+=` (Add and assign)
- `-=` (Subtract and assign)
- `*=` (Multiply and assign)
- `/=` (Divide and assign)

Example:
```java
int a = 5;
a += 10; // Equivalent to a = a + 10
a -= 3; // Equivalent to a = a - 3
```

#### 3.3 **Comparison Operators**

These operators compare two values and return a boolean value (`true` or `false`).

- `==` (Equal to)
- `!=` (Not equal to)
- `>` (Greater than)
- `<` (Less than)
- `>=` (Greater than or equal to)
- `<=` (Less than or equal to)

Example:
```java
int a = 5;
int b = 10;
boolean result = a == b; // false
result = a != b; // true
result = a > b; // false
```

#### 3.4 **Logical Operators**

Logical operators are used to combine multiple conditions.

- `&&` (Logical AND)
- `||` (Logical OR)
- `!` (Logical NOT)

Example:
```java
boolean condition1 = true;
boolean condition2 = false;
boolean result = condition1 && condition2; // false
result = condition1 || condition2; // true
result = !condition1; // false
```

---

### 4. **Example: Combining Variables and Operators**

```java
public class CombinedExample {
    public static void main(String[] args) {
        int x = 10;
        int y = 20;
        int sum = x + y; // Using arithmetic operator
        boolean isGreater = x > y; // Using comparison operator
        
        System.out.println("Sum: " + sum); // Output: Sum: 30
        System.out.println("Is x greater than y? " + isGreater); // Output: Is x greater than y? false
    }
}
```

**Output:**
```
Sum: 30
Is x greater than y? false
```

In this example:
- Arithmetic operator `+` is used to add `x` and `y`.
- Comparison operator `>` is used to check if `x` is greater than `y`.

---

### 5. **Conclusion**

Understanding sequence statements, variables, and operators in Java is fundamental to writing effective programs. By combining these elements, you can perform various operations, manipulate data, and control the flow of execution in your program.

Happy coding!
 