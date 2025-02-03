# Java Installation and Setup Guide

## Introduction
Java is a widely used programming language known for its platform independence and versatility. This guide will walk you through installing Java, setting up environment variables, and verifying your installation.

###### Step 1: Download Java
1. Visit the official [Oracle JDK download page](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html) or [OpenJDK](https://openjdk.org/).
2. Choose the version of Java suitable for your operating system.
3. Download and install the JDK (Java Development Kit).

###### Step 2: Set Up Environment Variables
**For Windows:**
1. Open the Start menu, search for `Environment Variables`, and open it.
2. Under "System Variables", find `Path`, and click `Edit`.
3. Click `New` and add the path to the Java `bin` directory (e.g., `C:\Program Files\Java\jdk-XX.X.X\bin`).
4. Click `OK` to save changes.

**For macOS/Linux:**
1. Open the terminal.
2. Edit your shell profile file (`~/.bashrc`, `~/.zshrc`, or `~/.bash_profile`) using a text editor.
3. Add the following lines:
   ```sh
   export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk-XX.X.X.jdk/Contents/Home
   export PATH=$JAVA_HOME/bin:$PATH
   ```
4. Save the file and apply changes with:
   ```sh
   source ~/.bashrc  # or source ~/.zshrc
   ```

###### Step 3: Verify Installation
To check if Java is installed correctly, open a terminal or command prompt and type:
```sh
java -version
```
You should see output displaying the installed Java version.

###### Step 4: Compile and Run a Java Program
Create a simple Java program to test the installation:
```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, Java!");
    }
}
```
Save the file as `HelloWorld.java`, then compile and run it:
```sh
javac HelloWorld.java
java HelloWorld
```
If everything is set up correctly, you should see:
```
Hello, Java!
```

## Conclusion
You have successfully installed and set up Java! You can now start building and running Java applications. 🚀
