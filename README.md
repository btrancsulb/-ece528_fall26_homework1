# -ece528_fall26_homework1
fahhhh


1a. A compiler translates the program into machine code before execution, while an interpreter translates and executes the instructions at runtime.

1b. By default, running main() will return a 0

2. Header files have shared declarations such as constants or structs, and The #include directive copies the contents of a header file into the source file before compilation.

3. To declare and define a function, you first declare the function using a function prototype. To define a function, you provide an implementation inside the function. For example:

   Function()
     {
     implementation
     }

The return statement sends a value back to the code that called the function and immediately terminates the function. The returned value must match the function’s return type. You can have more than one return statement.

4. Type casting converts a value from one data type to another. For example:

int add_as_int(double a, double b)
{
    return (int)(a + b);
}

5. Local variables are declared inside a function or block and can only be accessed there, whereas global variables are declared outside all functions and can be accessed by multiple functions in the same source file.

6. A string can be initialized using what is called a string literal. For example:
  char word[] = "Hello";

'\0', a null terminator, marks the end of the string. C string functions use it to know where the string ends.

7. Pointers are variables that store the memory address of another variable. A pointer is passed to a function by using a pointer parameter. For example:

void double_value(int *number)
{
    *number = *number * 2;
}

Passing a pointer allows a function to modify the original variable, avoid copying large data structures, return multiple results through output parameters, and work directly with arrays and dynamically allocated memory.

8. In the context of pointers, The & operator obtains the address of a variable and the * operator dereferences a pointer, accessing the value stored at its address.

9. A while loop checks its condition before executing, while do while loops execute the body first before checking its condition.

10. The break statement immediately exits the loop, but differs from a continue statement, because using continue skips the rest of the current iteration and begins the next iteration.

11. the & symbol is a bitwise AND operator
    the | Symbol is a bitwise OR operator
    the ^ symbol is a bitwise XOR operator
    the ~ symbol is for bitwise complement
    << is a bitwise shift to the left
    >> is a bitwise shift to the right

    To create a bit mask,
    
    uint8_t mask = (1 << 3);  // Binary: 00001000

    to set a bit using OR,

    value |= mask;

    to clear a bit,

    value &= ~mask;

    to toggle a bit,

    value ^= mask;

    to check a specific bit in an integer variable,

    if (value & mask)
