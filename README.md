# Bit Manipulation
Bit manipulation is the process of applying certain logical operations on a given sequence of bits to achieve the desired results. It can reduce the need to loop over a data structure and speed up the coding process as bit manipulations are processed in parallel.
The bits in the representation are indexed from right to left. 
We say that a certain bit is set, if it is one, and cleared if it is zero.
The binary number  (a<sub>k</sub>a<sub>k-1</sub>....a<sub>1</sub>a<sub>0</sub>)<sub>2</sub> represents the number
	(a<sub>k</sub>a<sub>k-1</sub>....a<sub>1</sub>a<sub>0</sub>)<sub>2</sub>=a<sub>k</sub>.2<sup>k</sup> + a<sub>k-1</sub>.2<sup>k-1</sup> + ... + a<sub>1</sub>.2<sup>1</sup> + a<sub>0</sub>.2<sup>0</sup> (in decimal)

| Operator | Name and Function of Operator | 
| -------- | ----------------------------- |
| & | Bitwise AND: The bitwise AND operator compares each bit of its first operand with the corresponding bit of its second operand. If both bits are 1, the corresponding result bit is set to 1. Otherwise, the corresponding result bit is set to 0. |
