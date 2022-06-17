# calculator-8051-assembly
A calculator using 8051 microprocessor, a numeric pad, a 2x16 LCD display and assembly code.

In this project, it was used Assembly language to implement a simple calculator using a numeric pad as input and a LCD display as output.

It was done using MCU 8051 IDE to write the code in Assembly and generate the hex file to put in Proteus schematic.

## Specifications

Since almost every register in 8051 is 8-bit, the calculator only works in the 0-255 range. It performs:

- Addition;
- Subtraction;
- Multiplication;
- Division;
- Reset the microprocessor and clean the LCD when 'ON/CE' is pressed.

It will show a error message (OVERFLOW!) if an input or an output is out of the 0-255 range, so negative numbers are not allowed either.
It will show another error message (DIV POR 0) if the user tries to divide by zero.
Another limitation is that it only works with two numbers. So, for example, if one tries to "1+2+3", when the '=' is typed, it will only do "1+3" because it's the last number and the first that the program will "remember".

The Assembly code is commented in Brazilian portuguese.
The .hex file is in the repo if you want to use only the simulation on Proteus (or similar).

![image](https://user-images.githubusercontent.com/69206952/174404173-d4b9634a-d077-4fe7-9f0c-c031b66adb63.png)

