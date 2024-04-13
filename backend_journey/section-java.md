# JAVA
On command prompt you use javac to check if the Java file is error free to generate byte code
**Public;** is use so the class can be accessed externally
**Static** is use so the jvm can know which object it is to call
**Void;** is a must to have in other to call the main method
**Main;** is a method and this apply to all major class. It’s comes with a bracket that entail what it should carry out (String args[]). The main method will compile but will not run without the String args[].
**System;** is a class
**Out** is an object
**.printl;** is a method and it follow a bracket of what is it to display (“hello world”).
**System.out.println(arg[0]);** it will print the argument stated alongside the string result.

### Video 5
***Import Java.lang.; ** is mandatory and even without type it. It is automatically in the code because of System.out.println().
It is best to have the file name and class name as the same tho have a different class name from file name is not a problem.
But when the class is declared public then the file name should be the same as the class name.

Video 6
Scanner works as a pipe to read the data from a keyboard.
Class Scanner
next() is use to read a string, that is one word
nextline() is use to read a couple of lines.
Class keybread;
Public static void main(String args[])
{        Scanner s=new scanner(system in);
String name
S.o.p (“May I know your name”);
name=s.nextline();
S.o.p (“I am” + name );
}.
Video 7
Scanner can’t work without importing Java.util*;
System.ln represent the keyboard
System.our represent the monitor
How to read keyboard using class scanner
Class keybread;
{
Public static void main(String args[])
{       
Scanner sc=new scanner(system in);
String x=sc.nextline ();
System.out.println(x);
}
}
Exceptions are runtime errors
For adding two numbers
Class keybread;
{
Public static void main(String args[])
{       
Scanner sc=new scanner(system in);
Int= a,b;
System.out.println(“enter two number”)
a =sc.nextint();
b =sc.nextint();
Int c=a+b;
System.out.pintln(“sun is” +z);
}
}.
To see all method available in scanner class on command prompt
Javap Java.util.scanner
For every data type,method is available.
We use radix for decimal numbers of 0 and 1
Class keyboard;
{
Public static void main(String args[])
{       
Scanner sc=new scanner(system in);
Sc.useradix(2);
Int x=sc.nextint ();
System.out.println(x);
}
}

Folder 2
Data types and variables
Variable are using for storing data
And the data makes up the program. It is an important part of a program
In Java,we have to first declare the variable and variable should have it data type
We have different type of data type
1 primitive data type;
It is subdivided into 3
Integral; they can have number with out decimal points. And are divided into 4.          i. Byte ii. Short iii. Int iv. Long
Boolean; they are not in number but true and false. While by default it is false.
Char; variable that represents letter
Float and double
Video 10
There are classes among these primitive data types
For every data type,there is a class available.
To check range and size for data type on command prompt is “javap java.lang.byte” or any data type.
Class datarangeandsize;
{
Public static void main(String args[])
{       
System.out.println(“int min” + Integral.Min_Value);
System.out.println(“int max” + Integral.Max_Value);
System.out.println(“int byte” + Integral.BYTE)
}
}
Video 11
VARIABLE
Variable are name given to data and to store data
Initialising variables you will add a value.
To declare variables
Data type name and the name of variable then you initialise by adding number.
If a value is beyond the range of a data type,it’s will bring error.
Class variables;
{
Public static void main(String args[])
{       
Int I= 100;
Char c= ‘A’;
System.out.println(I);
System.out.println(c);
}
}
Video 12
Variable — Naming Rule
Case sensitive ; two variables cannot have same names written same way.
Variable name should not have key word
It can only start with alphabet,_,$
Contain Alphabet,number,_ or $
Don’t use class name
There is no limit on variable name
Space between a variable name is not allowed so there must be an ‘_’
A number cannot be a starting variable name.
Follow camel cases; the first word start with a small letter then the word that follow should be in capital “rollNumber”. And camel case are use instead of using_ and $
Literal
They are those constant values that are used in a program.
Literal have their data type
Integer literal; 5,6,24
Double literal; 3.1425,153.45
Char literal; ‘A’
String literal; “Java”
How to declare literal
Byte,short and int are all declare int
Long are declared with L & l
Float ; F & f
Double; D & d
Char; ‘’
Boolean; true or false
For long number,you can use _to separate the number and don’t add _ at the end
How to represent negative forms
1 represents negative sign
0 represents positive sign
For small number it is best to use byte and short to save space and run quickly.
How to print number in binary form
For int you use system.out.println(Integer.tobinarystring(x));
It’s only works for integers
Folder 4
Interpreter and Compliler
They are translations
Compiler execute once and you can run your as many time are possible and it is faster. When running your program,jvm is running.
Javac is just turning it to machine code
Interpreter language are easier to learn but takes time to run
How Java are Executed and platform independent.
Source code — javac and convert it to byte code and error free —— jvm and it has an interpreter and JIT compiler. It will concern it to  machine code. It will be executed on operating system. Program execute using operating system. Jvm can interpret byte code and talk to operating system.
Jvm can talk to different operating systems. Once Java code are compile,you can run on any platform. Byte code and jvm makes it platform independent.
While cc++ you can create code on a window and cannot execute on Mac unlike Java.
On cpp or c++
Exe can only work on window. A program compile on windows cannot work on Mac
Architecture of JVM
Requirements for running any program.
Memory

Method Area;Where the program reside. Class loading is done by class loader. It’s stores online method. JIT compiler will execute the code.
Stack; variable are created in the stack.
Heap; springs object are created in the heap. Anything object by saying new is saved in heap. Whenever a method is called a stack firm is created.
7:59
Component of JVM Memory
Class loader
Stack
Heap
Method area
Execution engine; Garbage collector take object that are not used in heap.javac
Pc register
The method done in c++ are called native method. They are external method but jvm are responsible for them
Class loader
They are divided in 3
Loading; it has 3 class loader I.Bootstrap are used for loading Java sc classes. ii. External; they provide runtime environment for jvm. Bootstrap and external will load the run time class that are provided by jvm. iii. Application class loader— it load our own application.
Linking: I. Verify; it check if the byte code is secure and correct or not ii. Prepare; it create memory for static variables that are stored in method area. iii. Resolve; it is the main method for linking.
Initialisation; it’s initialise static variables and it’s execute static block.
### STACK
Each thread will have their own stack area but all threads will use same heap area.

### PC REGISTERS
Each thread should have their own Pc register

## EXECUTION ENGINE

Interpreter; it’s changed byte code to machine code

JIT COMPILER; machine code is converted only once.
Garbage collector; if there is an unused object in the heap area,garbage collector will collect it.

NATIVE METHOD INTERFACE
It will all native method to communicate with jvm.

NATIVE METHOD LIBRARY

NATIVE METHOD STACK

## FEATURE IN JAVA

Simple

Secure; it’s can get infected by virus. Java  runs within the shell of jvm so there is not room for virus.

Portable; it’s can move from one platform to another. Platform independent

Object Oriented are very easy to learn

Robust; they are very strong. In lack of resources,it’s wouldn’t clash and that is we have exception handling

Multithreaded

Architecture Neutral; Vin-Neumann architecture. ARM can be use on phone

Interpreted language; javac made it fast it is low but of high performance
High performance

Distributed

Dynamic


# Folder 5
## OPERATION AND EXPRESSION

Arithmetic operations; its can’t be operated on Boolean. “,/,%” have higher precidence than + and -. () are use if you are using +and-.
Coacion is a conversion done internally
Int + short = int
F+d  = double
Int + float = f


Folder 6
## PRINTING
System; stands for the class
Out; stands for the object and link to the monitor
Println; is a method. It’s will print and move to the next line.
While print; is another method but will not move to the next line.
Println; are also all loaded. They can take all type of parameter.
You can add expressions in the parameter
Printf; you need to add \n to parameters so there can be a space after printing
Fromat; also the way printf is

### FORMAT SPECIFICATIONS
%
Conversion; for Float —— f,e,g. Int—— d”decimal” o “octal” x “haze decimal representation number 1-7 and letter a-h”. String — s, Char— c.
Argument index; 1$,2$,3$.
Flag; if the number is negative and the %and conversion has a bracket it’s wil be in bracket. For float with most time save in nearest number

## STRING
String is a class of characters that can form a word
String — class
Str —— method
“Word” — string object
