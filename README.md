# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  

# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof() :
  
   3.1 Integer literal (e.g., 10) using `%d`
   
   3.2 Float literal (e.g., 3.14) using `%f`
   
   3.3 Character literal (e.g., 'A') using `%c`
   
   3.4 String literal (e.g., "Hello C") using `%s`
   
### Step 4: 
   Stop
# Program:
```
#include <stdio.h>
int main() {
    printf("Size of integer literal %d is: %zu bytes\n", 10, sizeof(10));
    printf("Size of float literal %f is: %zu bytes\n", 3.14, sizeof(3.14));
    printf("Size of character literal '%c' is: %zu bytes\n", 'A', sizeof('A'));
    printf("Size of string literal \"%s\" is: %zu bytes\n", "Hello C", sizeof("Hello C"));
    return 0;
}
```
# Output:
<img width="505" height="242" alt="image" src="https://github.com/user-attachments/assets/6f5814ec-f858-450d-86d1-0adc4ec6533b" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.

# Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
# Algorithm:
### Step 1:
  Start  
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Define a macro constant `PI` with value `3.14159` using `#define`.
### Step 4: 
   Inside `main()`:
   
   4.1 Declare a constant integer variable `DAYS`
   
   4.2 Initialize it with the value `7`
   
### Step 5:  
  Use `printf()` to display the values of `PI` and `DAYS`.     
### Step 6:  
  Stop
# Program:
```
#include <stdio.h>
#define PI 3.14159
int main() {
    const int DAYS = 7;
    printf("Value of PI is: %f\n", PI);
    printf("Value of DAYS is: %d\n", DAYS);
    return 0;
}
```
# Output:
<img width="418" height="232" alt="image" src="https://github.com/user-attachments/assets/2a09b077-1ac1-416f-8a8e-5cccf88e0812" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().

# Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside main(), declare and initialize variables of types int, float, double, and char.
### Step 4: 
   Display their values using printf().
### Step 5:    
   Stop
# Program:
```
#include <stdio.h>
int main() {
    int a = 25;
    float b = 98.6f;     
    double c = 3.14159265;
    char d = 'A';
    printf("Integer value: %d\n", a);
    printf("Float value: %f\n", b);
    printf("Double value: %lf\n", c);
    printf("Character value: %c\n", d);
    return 0;
}
```
# Output:
<img width="368" height="261" alt="image" src="https://github.com/user-attachments/assets/40babb3c-89e0-4db4-9e4b-785401b52442" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare two integer variables a and b.
### Step 4: 
   Prompt the user to enter two integers and read the input using scanf().
### Step 5:    
   Perform arithmetic operations on a and b:
   #### Sum (a + b)
   #### Difference (a - b)
   #### Product (a * b)
   #### Quotient (a / b)
   #### Remainder (a % b)
### Step 6: 
  Perform bitwise operations on a and b:
  #### AND (a &amp; b)
  #### OR (a | b)
  #### XOR (a ^ b)
  #### Left shift (a << b)
  #### Right shift (a >> b)
  #### Bitwise NOT of a (~a) and b (~b)
### Step 7:   
  Display the results of all operations using printf().
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>
int main() {
    int a, b;
    printf("Enter two integers (a and b): ");
    scanf("%d %d", &a, &b);
    printf("\nArithmetic Operations:\n");
    printf("Sum (a + b)       = %d\n", a + b);
    printf("Difference (a - b)= %d\n", a - b);
    printf("Product (a * b)   = %d\n", a * b);
    if (b != 0) {
        printf("Quotient (a / b)  = %d\n", a / b);
        printf("Remainder (a %% b) = %d\n", a % b); 
    } 
    else 
    {
        printf("Quotient (a / b)  = Undefined (Cannot divide by zero)\n");
        printf("Remainder (a %% b) = Undefined (Cannot divide by zero)\n");
    }

    printf("\n Bitwise Operations:\n");
    printf("AND (a & b)       = %d\n", a & b);
    printf("OR (a | b)        = %d\n", a | b);
    printf("XOR (a ^ b)       = %d\n", a ^ b);
    printf("Left shift (a << b)  = %d\n", a << b);
    printf("Right shift (a >> b) = %d\n", a >> b);
    printf("Bitwise NOT of a (~a)= %d\n", ~a);
    printf("Bitwise NOT of b (~b)= %d\n", ~b);
    return 0;
}
```
# Output:
<img width="473" height="653" alt="image" src="https://github.com/user-attachments/assets/e9f511f4-7422-4859-8676-8b532e26dc42" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Input a character ch from the user.
### Step 4: 
   Check if ch is a digit ('0' to '9').
   
   If true → Print "Digit" → Go to Step 8.
   
   If false → Go to Step 5.
   
### Step 5:    
   Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').
   
   If true → Go to Step 6.
   
   If false → Go to Step 7.
   
### Step 6: 
   Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).
   
   If true → Print "Vowel" → Go to Step 8.
   
   If false → Print "Consonant" → Go to Step 8.
   
### Step 7:   
   Print "Special Symbol".
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>
int main() {
    char ch;
    printf("Enter a single character: ");
    scanf("%c", &ch);
    (ch >= '0' && ch <= '9') ? 
        printf("Digit\n") :
        ( (ch >= 'a' && ch <= 'z') || (ch >= 'A' && ch <= 'Z') ) ? 
            
            ( (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u' || 
               ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U') ? 
                printf("Vowel\n") :      
                printf("Consonant\n")    
            ) 
            : printf("Special Symbol\n");  
    return 0;
}
```
# Output:
<img width="368" height="197" alt="image" src="https://github.com/user-attachments/assets/3f35d689-1700-47f6-a02e-0ed0765ab58b" />
<img width="397" height="223" alt="image" src="https://github.com/user-attachments/assets/d81fb765-5ca4-4198-9aa6-1ed1d4910f3f" />
<img width="393" height="220" alt="image" src="https://github.com/user-attachments/assets/83e28a5e-c192-4190-a400-e7776074377c" />


# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


