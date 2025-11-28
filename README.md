Exception Handling Program

A simple Java program demonstrating the core concepts of exception handling, including:

try, catch, and finally blocks

Using throw to manually throw exceptions

Using throws to declare exceptions

This program helps beginners understand how Java handles runtime errors and ensures robust and predictable program flow.

📌 Features
✔️ Try–Catch–Finally

try block contains code that may cause an exception.

catch block handles the exception gracefully.

finally block executes regardless of whether an exception occurs (useful for cleanup tasks like closing files or connections).

✔️ Throw

Demonstrates manually throwing an exception using the throw keyword.

✔️ Throws

Demonstrates declaring checked exceptions in a method signature using throws.

📁 Project Structure
ExceptionHandlingDemo/
 ├── src/
 │    ├── Main.java
 │    ├── ThrowExample.java
 │    └── ThrowsExample.java
 └── README.md

📝 Example Code Snippet
Try–Catch–Finally
try {
    int result = 10 / 0;  
} catch (ArithmeticException e) {
    System.out.println("An error occurred: " + e.getMessage());
} finally {
    System.out.println("Finally block executed.");
}

Throw Example
public void validateAge(int age) {
    if (age < 18) {
        throw new IllegalArgumentException("Age must be 18 or above.");
    }
}

Throws Example
public void readFile() throws IOException {
    FileReader fr = new FileReader("data.txt");
}

▶️ How to Run the Program

Clone or download this project.

Open it in any Java IDE (VS Code, IntelliJ, Eclipse) or compile via command line.

Run:

javac Main.java
java Main
