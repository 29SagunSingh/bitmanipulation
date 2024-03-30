# Bit Manipulation
Bit manipulation is the process of applying certain logical operations on a given sequence of bits to achieve the desired results. It can reduce the need to loop over a data structure and speed up the coding process as bit manipulations are processed in parallel.
The bits in the representation are indexed from right to left. 
We say that a certain bit is set, if it is one, and cleared if it is zero.
The binary number  (a<sub>k</sub>a<sub>k-1</sub>....a<sub>1</sub>a<sub>0</sub>)<sub>2</sub> represents the number 
	a<sub>k</sub>.2<sup>k</sup> + a<sub>k-1</sub>.2<sup>k-1</sup> + ... + a<sub>1</sub>.2<sup>1</sup> + a<sub>0</sub>.2<sup>0</sup> (in decimal)

 ###Pre-requisites:
 ##Binary Number System
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

###Binary Number Table
![image](https://github.com/29SagunSingh/bitmanipulation/assets/143775654/37f7457d-bcef-4165-a185-664f1ea91f75)
![image](https://github.com/29SagunSingh/bitmanipulation/assets/143775654/74fd43c0-6c79-44f3-acfb-801531147073)



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
