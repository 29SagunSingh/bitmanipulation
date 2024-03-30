# Bit Manipulation
Bit manipulation is the process of applying certain logical operations on a given sequence of bits to achieve the desired results. It can reduce the need to loop over a data structure and speed up the coding process as bit manipulations are processed in parallel.
The bits in the representation are indexed from right to left. 
We say that a certain bit is set, if it is one, and cleared if it is zero.
The binary number  (a<sub>k</sub>a<sub>k-1</sub>....a<sub>1</sub>a<sub>0</sub>)<sub>2</sub> represents the number 
	a<sub>k</sub>.2<sup>k</sup> + a<sub>k-1</sub>.2<sup>k-1</sup> + ... + a<sub>1</sub>.2<sup>1</sup> + a<sub>0</sub>.2<sup>0</sup> (in decimal)

### Pre-requisites:
## Binary Number System
 Binary Number System is a number system that is used to represent various numbers using only two symbols “0” and “1”. The word binary is derived from the word “bi” which means two. Hence, this number system is called Binary Number System. Thus, the binary number system is a system that has only two symbols.
There are generally various types of number systems and among them the four major ones are,
•	Binary Number System (Number system with Base 2)
•	Octal Number System (Number system with Base 8)
•	Decimal Number System (Number system with Base 10)
•	Hexa decimal Number System (Number system with Base 16

![image](https://github.com/29SagunSingh/bitmanipulation/assets/143775654/c6306bab-eb64-4803-8635-6debb7c10f6e)

  In the Binary Number System, we have a base of 2. The base of the Binary Number System is also called the radix of the number system.
In a binary number system, we represent the number as,
•	(11001)2
In the above example, a binary number is given in which the base is 2. In a binary number system, each digit is called the “bit”. In the above example, there are 5 digits.

### Binary Number Table
![image](https://github.com/29SagunSingh/bitmanipulation/assets/143775654/37f7457d-bcef-4165-a185-664f1ea91f75)
![image](https://github.com/29SagunSingh/bitmanipulation/assets/143775654/74fd43c0-6c79-44f3-acfb-801531147073)

### Binary to Decimal Conversion
A binary number is converted into a decimal number by multiplying each digit of the binary number by the power of either 1 or 0 to the corresponding power of 2. Let us consider that a binary number has n digits, B = a<sub>n-1</sub>…a<sub>3</sub>a<sub>2</sub>a<sub>1</sub>a<sub>0</sub>. Now, the corresponding decimal number is given as
![image](https://github.com/29SagunSingh/bitmanipulation/assets/143775654/6e46fae3-4a4f-4211-83bd-f1f04355fd88)

##### Example: Convert (10011)<sub>2</sub> to a decimal number.
![image](https://github.com/29SagunSingh/bitmanipulation/assets/143775654/64b3b843-088e-4115-bf26-62691705e2ed)

### Decimal to Binary Conversion
A decimal number is converted into a binary number by dividing the given decimal number by 2 continuously until we get the quotient as 1, and we write the numbers from downwards to upwards.
###### Example: Convert (28)<sub>10/<sub> into a binary number.
![image](https://github.com/29SagunSingh/bitmanipulation/assets/143775654/08b90d65-76e7-47a1-b2d0-d9289cc1ddb5)

### Arithmetic Operations on Binary Numbers
We can easily perform various operations on Binary Numbers. Various arithmetic operations on the Binary number include,
•	Binary Addition
•	Binary Subtraction
•	Binary Multiplication
•	Binary Division

#### Binary Addition
The result of the addition of two binary numbers is also a binary number. To obtain the result of the addition of two binary numbers, we have to add the digit of the binary numbers by digit. The table added below shows the rule of binary addition.
![image](https://github.com/29SagunSingh/bitmanipulation/assets/143775654/80909ad1-2612-405e-9007-793f09d41ab8)

#### Binary Subtraction
The result of the subtraction of two binary numbers is also a binary number. To obtain the result of the subtraction of two binary numbers, we have to subtract the digit of the binary numbers by digit. The table added below shows the rule of binary subtraction.
![image](https://github.com/29SagunSingh/bitmanipulation/assets/143775654/4ee1ca3f-3d4a-49ec-867c-d438b28d44e6)

#### Binary Multiplication
The multiplication process of binary numbers is similar to the multiplication of decimal numbers. The rules for multiplying any two binary numbers are given in the table.
![image](https://github.com/29SagunSingh/bitmanipulation/assets/143775654/f3ea558b-af45-4e05-b1d2-a2cca3d9e375)



| Operator | Name and Function of Operator | 
| -------- | ----------------------------- |
| & | Bitwise AND: The bitwise AND operator compares each bit of its first operand with the corresponding bit of its second operand. If both bits are 1, the corresponding result bit is set to 1. Otherwise, the corresponding result bit is set to 0. |
| | | Bitwise OR: The bitwise inclusive OR operator compares each bit of its first operand with the corresponding bit of its second operand. If one of the two bits is 1, the corresponding result bit is set to 1. Otherwise, the corresponding result bit is set to 0. |
| ~ | One’s complement / NOT: The bitwise complement (NOT) operator flips each bit of a number, if a bit is set the operator will clear it, if it is cleared the operator sets it. |
| ^ | Bitwise XOR: The bitwise exclusive OR (XOR) operator compares each bit of its first operand with the corresponding bit of its second operand. If one bit is 0 and the other bit is 1, the corresponding result bit is set to 1. Otherwise, the corresponding result bit is set to 0. |
| << | Left shift: Shifts a number to the left by appending zero digits. A left shift by k represents a multiplication by  2^k. |
| >> | Right shift: Shifts a number to the right by removing the last few binary digits of the number. Each shift by one represents an integer division by 2, so a right shift by k represents an integer division by 2^k. |

## Get the bit at a specific position
To find the bit at position i in a given number N, you can perform a bitwise AND operation between N and 2 raised to the power of i (represented as (1 << i)). This operation checks whether the bit at position i is set or unset. If the resulting value is 1, then the bit at position i is set. Otherwise, it is unset.

bool getBit(int num, int i)
{
    // Return true if the bit is
    // set. Otherwise, return false
    return ((num & (1 << i)) != 0);
}
