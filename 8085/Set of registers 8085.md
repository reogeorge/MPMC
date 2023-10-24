It consists of several registers including 
- 8 bit [[#Accumulator|accumulator]]
- six 8 bit [[#General purpose registers|general purpose registers]]
- 16 bit [[#Stack pointer|stack pointer]]
- 16 bit [[#Program counter|program counter]]
- 8 bit [[#Instruction Register]]
- 8 bit [[#Temporary Register]]
- [[Flags 8085|Flags]]

# Accumulator

The Accumulator stores one of the operands for an arithmetic or logical operation, the other may be stored in a register or in memory.

The [[ALU 8085|arithemetic/logical operation]] is performed in the ALU and the result is stored the Accumulator
# General Purpose Registers

There are 6 general purpose registers in [[8085 Intel|8085]]. 
They are of 8 bit in size.
They are **B C D E H L**.

To Store 16 bit data, the registers are combined as a pair, the pairing is pre done and cannot be choosen by the programmer 
	the pairings are as follows
		B-C 
		D-E
		H-L
			the H-L pair is used to act as a memory pointer.

The general purpose registers and accumulator can be used by a programmer to store data into.

# Stack Pointer

It is a special register used to store the address of the top element in a [[Stack]] 
Stack can store contents of accumulator, general purpose...
The stack and stack pointer are initialized by the programmer.
example
	when the microprocessor jumps to a subroutine, the contents of program counter is stored into stack
# Program counter

The program counter stores the memory address of the next instruction to be executed.
	During the execution of an instruction 8086 increments the Program counter so as to make it point to the next instruction to be executed.


# Instruction Register

Stores the [[Opcode|opcode]] of the instruction which is being decoded and executed.


# Temporary Register

Associated with [[ALU 8085|ALU]], not accessible by programmer.

