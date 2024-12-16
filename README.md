# Cpp

### Introduction
The C language was developed in 1972 by Dennis Ritchie, primarily as a systems programming language.  
C++ was developed by Bjarne Stroustrup at Bell Labs as an extension to C, starting in 1979.  

#### What is C++ good at?
* Video games
* Real-time systems (e.g. for transportation, manufacturing, etc…)
* High-performance financial applications (e.g. high frequency trading)
* Graphical applications and simulations
* Productivity / office applications
* Embedded software
* Audio and video processing
* Artificial intelligence and neural networks

#### The Development Process
1. Define the problem to solve
    * "I want to write a program that ..."
2. Design a solution
    * straightforward
    * well documented
    * built modularly
    * recover from errors and provide helpful messages
3. Write a program that implements the solution
4. Compile the program
5. Link object files
6. Test program
7. Debug

#### Common Problems
1. General run-time issues
   * When executing a program, the console window blinks and then closes immediately.  
Add or ensure the following are near the top of the program:
```{C++}
// after #include "pch.h" or #include "stdafx.h" if present
#include <iostream>
#include <limits>
```
Add the following at the end of the `main()` function right before the return statement:
```{C++}
std::cin.clear(); //reset any error flag
std::cin.ignore(std::numeric_limits<std::streamsize>::max(), '\n'); // ignore any characters in the input buffer until we find an enter character
std::cin.get(); // get one more char from the user
```
  * Running program opens window but no output.
Check virus scanner or anti-malware.
2. General compile-time issues
  * When I compile, I get an error about unresolved external symbol _main or _WinMain@16
      * This means compiler can't find the main() function
      * Does your code include a function named main()?
      * Is main spelled correctly?
Actually, refer to documentation, check error codes on search engines, look at [Learn C++](https://www.learncpp.com/cpp-tutorial/a-few-common-cpp-problems/).

### Statements and Structure
There are many different kinds of statements in C++:
1. Declaration
2. Jump
3. Expression
4. Compound
5. Selection statements (conditionals)
6. Iteration
7. Try blocks






