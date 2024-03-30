# Bit Manipulation
Bit manipulation is the process of applying certain logical operations on a given sequence of bits to achieve the desired results. It can reduce the need to loop over a data structure and speed up the coding process as bit manipulations are processed in parallel.
The bits in the representation are indexed from right to left. 
We say that a certain bit is set, if it is one, and cleared if it is zero.
The binary number  (a<sub>k</sub>a<sub>k-1</sub>....a<sub>1</sub>a<sub>0</sub>)<sub>2</sub> represents the number
	(a<sub>k</sub>a<sub>k-1</sub>....a<sub>1</sub>a<sub>0</sub>)<sub>2</sub>=a<sub>k</sub>.2<sup>k</sup> + a<sub>k-1</sub>.2<sup>k-1</sup> + ... + a<sub>1</sub>.2<sup>1</sup> + a<sub>0</sub>.2<sup>0</sup> (in decimal)

| Operator | Name and Function of Operator | 
| -------- | ----------------------------- |
| & | Bitwise AND: The bitwise AND operator compares each bit of its first operand with the corresponding bit of its second operand. If both bits are 1, the corresponding result bit is set to 1. Otherwise, the corresponding result bit is set to 0. |
| | | Bitwise OR: The bitwise inclusive OR operator compares each bit of its first operand with the corresponding bit of its second operand. If one of the two bits is 1, the corresponding result bit is set to 1. Otherwise, the corresponding result bit is set to 0. |
| ~ | One’s complement / NOT: The bitwise complement (NOT) operator flips each bit of a number, if a bit is set the operator will clear it, if it is cleared the operator sets it. |
| ^ | Bitwise XOR: The bitwise exclusive OR (XOR) operator compares each bit of its first operand with the corresponding bit of its second operand. If one bit is 0 and the other bit is 1, the corresponding result bit is set to 1. Otherwise, the corresponding result bit is set to 0. |
| << | Left shift: Shifts a number to the left by appending zero digits. A left shift by k represents a multiplication by  2^k. |
| >> | Right shift: Shifts a number to the right by removing the last few binary digits of the number. Each shift by one represents an integer division by 2, so a right shift by k represents an integer division by 2^k. |
