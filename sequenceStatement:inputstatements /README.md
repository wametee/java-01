
# Sequence Statements: Input Statements (Using Scanner, BufferedReader) in Java

### Introduction
In Java, input statements allow the program to receive data from the user. This is typically done using `Scanner` and `BufferedReader`. The input received can be of different types, such as integers, strings, or floating-point numbers. This README discusses how to use `Scanner` and `BufferedReader` for input handling in Java.

---

### 1. **Using Scanner for Input in Java**

The `Scanner` class is part of the `java.util` package and is commonly used to take input from the user via the console. It supports different types of inputs such as integers, strings, and floating-point numbers.

#### 1.1 **Scanner Class Example**

To use `Scanner`, first import the class and then create an object of the `Scanner` class.

```java
import java.util.Scanner;

public class ScannerExample {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Reading an integer
        System.out.print("Enter an integer: ");
        int num = scanner.nextInt();

        // Reading a string
        System.out.print("Enter a string: ");
        String str = scanner.next();

        System.out.println("You entered the integer: " + num);
        System.out.println("You entered the string: " + str);
    }
}
```

**Output:**
```
Enter an integer: 25
Enter a string: Hello
You entered the integer: 25
You entered the string: Hello
```

#### 1.2 **Commonly Used Methods in Scanner**

- `nextInt()`: Reads an integer.
- `nextLine()`: Reads a full line of text.
- `nextDouble()`: Reads a double.
- `next()`: Reads a single word (delimited by spaces).

Example of reading different types of inputs:
```java
Scanner scanner = new Scanner(System.in);

int num = scanner.nextInt();
double decimal = scanner.nextDouble();
String str = scanner.nextLine();
```

---

### 2. **Using BufferedReader for Input in Java**

`BufferedReader` is another method to read input in Java. It is used to read text from a character-based input stream, such as the console. The `BufferedReader` class is part of `java.io` package and is generally faster than `Scanner` when reading large inputs because it buffers characters for efficient reading.

#### 2.1 **BufferedReader Class Example**

```java
import java.io.*;

public class BufferedReaderExample {
    public static void main(String[] args) throws IOException {
        BufferedReader reader = new BufferedReader(new InputStreamReader(System.in));

        // Reading a string
        System.out.print("Enter a string: ");
        String str = reader.readLine();

        // Reading an integer
        System.out.print("Enter an integer: ");
        int num = Integer.parseInt(reader.readLine());

        System.out.println("You entered the string: " + str);
        System.out.println("You entered the integer: " + num);
    }
}
```

**Output:**
```
Enter a string: Java
Enter an integer: 50
You entered the string: Java
You entered the integer: 50
```

#### 2.2 **Key Methods in BufferedReader**

- `readLine()`: Reads a line of text.
- `parseInt()`, `parseDouble()`, etc.: These methods can be used to convert string input into the desired numeric data types.

Example of converting input:
```java
BufferedReader reader = new BufferedReader(new InputStreamReader(System.in));

String str = reader.readLine();
int num = Integer.parseInt(reader.readLine());
```

---

### 3. **Comparison Between Scanner and BufferedReader**

| Feature               | Scanner                         | BufferedReader                 |
|-----------------------|---------------------------------|---------------------------------|
| **Package**           | `java.util.Scanner`             | `java.io.BufferedReader`        |
| **Type of Input**     | Can read various types (int, string, double, etc.) | Primarily reads strings |
| **Speed**             | Slower compared to BufferedReader | Faster when reading large input |
| **Handling Newlines** | Handles newlines with `nextLine()` method | Handles newlines with `readLine()` method |
| **Error Handling**    | Can throw exceptions (InputMismatchException, etc.) | Can throw IOException |

- **Scanner** is easier to use for various types of input, including numbers and strings.
- **BufferedReader** is better for reading large amounts of text efficiently.

---

### 4. **Example: Combining Both Input Methods**

```java
import java.io.*;
import java.util.Scanner;

public class CombinedInputExample {
    public static void main(String[] args) throws IOException {
        // Using Scanner
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a double number: ");
        double d = scanner.nextDouble();
        
        // Using BufferedReader
        BufferedReader reader = new BufferedReader(new InputStreamReader(System.in));
        System.out.print("Enter a string: ");
        String str = reader.readLine();

        System.out.println("You entered the double: " + d);
        System.out.println("You entered the string: " + str);
    }
}
```

**Output:**
```
Enter a double number: 3.14
Enter a string: Hello BufferedReader
You entered the double: 3.14
You entered the string: Hello BufferedReader
```

---

### 5. **Conclusion**

Both `Scanner` and `BufferedReader` are used to take input from users in Java. `Scanner` is more versatile for reading different types of input, while `BufferedReader` is often preferred for reading large inputs efficiently. Understanding when and how to use each input method is essential for writing robust Java applications.

Happy coding!
