# Java Programming Notes

## Programming Paradigm

1. **Procedural Programming**
2. **Functional Programming**
3. **Object-Oriented Programming**

---

## Compilation of Code

```
.java  ----->  .class (byte code)  ----->  machine code
       javac                    JVM
```

---

## Components of JVM

* **Class Loader**
* **Memory Area**
* **Execution Engine**

  * Interpreter
  * JIT (Just-In-Time) Compiler
* **Garbage Collection**

---

## JVM → JRE → JDK

* **JVM (Java Virtual Machine)** → Executes Java bytecode.
* **JRE (Java Runtime Environment)** → JVM + standard libraries required for execution.
* **JDK (Java Development Kit)** → JRE + compiler and development tools.

---

## Everything in Java is Written in Classes

A **class** is a user-defined blueprint having **attributes** and **methods**.

Example:

```
class Example {
    int num;             // attribute
    void display() {     // method
        System.out.println(num);
    }
}
```

---

## The main() Method

```
public static void main(String[] args) { }
```

| Component         | Description                                            |
| ----------------- | ------------------------------------------------------ |
| **public**        | Access modifier, visible to all.                       |
| **static**        | Allows calling the method without creating an object.  |
| **void**          | Return type — does not return a value.                 |
| **main**          | Entry point of the Java program.                       |
| **String[] args** | Default command-line argument list (array of strings). |

---

## Example Program

```
class HelloWorld {
    public static void main(String[] args) {
        System.out.println(args[0]);
    }
}
```

### Compilation Steps

```
javac HelloWorld.java
java HelloWorld arg_1 arg_2
```

---

## System.out.println() Explanation

`System.out.println()` → Prints the output and then creates a new line for the next output.

| Component   | Description                                                              |
| ----------- | ------------------------------------------------------------------------ |
| **System**  | Predefined class providing access to input, output, and error streams.   |
| **out**     | Object of the `PrintStream` class.                                       |
| **println** | Method in `PrintStream` class that prints output followed by a new line. |

Example:

```
System.out.print("Hello Java");
System.out.println(args[0]);
```

**Output:**

```
Hello Javaarg_1
```

---

### Notes

* `System.out.print()` → Prints the output **without** moving to a new line.
* `System.out.println()` → Prints the output **and moves** to a new line.

---
