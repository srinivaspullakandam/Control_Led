Control LED with Control Board

Need help? Contact support@freenove.com █
Code Knowledge
Before start writing code, we should learn about the basic programming knowledge.

Comments
Comments are the words used to explain for the sketches, and they won't affect the running of code.
There are two ways to use comments of sketches.
1.
Symbol "//"
Contents behind ”//” comment out the code in a single line.

1 // this is a comment area in this line.
The content in front of "//" will not be affected. 1 delay(1000); // wait for a second
2.
Symbol "/*"and "*/"
Code can also be commented out by the contents starting with a “/*” and finishing with a “*/” and you can place it anywhere in your code, on the same line or several lines. 1 /* this is comment area. */
Or 1 2 3 4 /* this is a comment line. this is a comment line. */

Data type
When programming, we often use digital, characters and other data. C language has several basic data types as follows:
int: A number that does not have a fractional part, an integer, such as 0, 12, -1;
float: A number that has a fractional part, such as 0.1, -1.2;
char: It means character, such as 'a', '@', '0';
For more about date types, please visit the website: https://www.Arduino.cc-Resources-Reference-Data Types.
Constant
A constant is a kind of data that cannot be changed, such as int type 0, 1, float type 0.1, -0.1, char type 'a', 'B'.
Variable
A variable is a kind of data that can be changed. It consists of a name, a value, and a type. Variables need to be defined before using, such as:


1 int i;
"int" indicates the type, ";" indicates the end of the statement. The statement is usually written in one single line; and these statements form the code.
After declaration of the variable, you can use it. The following is an assignment to a variable: 1 i = 0; // after the execution, the value of i is 0
"=" is used to pass the value of a variable or constant on the right side to the variable on the left.

A certain number of variables can be declared in one statement, and a variable can be assigned multiple times. Also, the value of a variable can be passed to other variables. For example:

1 2 3 4 int i, j; i = 0; // after the execution, the value of i is 0 i = 1; // after the execution, the value of i is 1 j = i; // after the execution, the value of j is 1
Function
A function is a collection of statements with a sequence of order, which performs a defined task. Let's define a function void blink() as follows:

void blink() { digitalWrite(13, HIGH); delay(1000); digitalWrite(13, LOW); delay(1000); }


"void" indicates that the function does not return a value (Chapter 4 will detail the return value of functions);
"()" its inside is parameters of a function (Chapter 2 will detail the parameters of the functions). No content inside it indicates that this function has no parameters;
"{}" contains the entire code of the function.
After the function is defined, it is necessary to be called before it is executed. 
