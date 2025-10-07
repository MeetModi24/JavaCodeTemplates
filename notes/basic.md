Programming Paradigm
1) Procedural Programming
2) Functional Programming
3) Object Oriented Programming

Compilation of code
.java  -----> .class(byte code) -----> machine code
       javac                    JVM

Components of JVM: Class Loader, Memory area, Execution engine: Interpreter, JIT compiler, Garbage collection

JVM-->JRE-->JDK

Everything in JAVA is written in classes.
class- a user defined blueprint having attributes and methods

public static void main(String[] args){} --> is a function(method)
Return type of function: void
Function name: main --> entry point of java program
public : access modifier, visible to all
static : allows us to call the functions, methods without creating object of class.
String[] args: default command line arguments string list

Eg. javac Main.java
java Main arg_1 arg_2

class HelloWorld{
    public static void main(String[] args){
        System.out.println(args[0]);
    }
}

Compilation step:
javac HelloWorld.java
java HelloWorld arg_1 arg_2


System.out.println() --> print the output and then create new line for next
System : class present by default providing input, output, and error methods
out : object of class PrintStream class
println : method in PrintStream class

System.out.print("Hello Java");
System.out.println(args[0]);
Output: Hello Javaarg_1

