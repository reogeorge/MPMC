
![[Flags 8085.png]]

In 8085, 5 flip flops serve as status flags, these flags are set or reset based of the result obtained from the [[ALU 8085|ALU]] operations. The combination of values in the 8 flags(5+3) is known as 
*program status word*.
The program status word along with the value in accumulator is used for [[Stack|stack]] operations.

# Sign(S)

The sign bit is set to 0 if the result of [[ALU 8085|ALU]] operations is positive, else its set as 0.
The [[MSB|MSB]] is used to know the sign here.


# Zero(Z)

Zero flag is set if the result of a [[ALU 8085]] is 0



# Auxiliary carry flag(AC)

This carry is set to 1 only if a carry is sent from 3rd bit to 4th bit.



# Parity(P)

It is set if the number of 1s of the result is even and reset if odd


# Carry(CY)

If the result of the [[ALU 8085|Arithemetic operation]] is more than 8 bits then the [[MSB]] of the result is stored in the carry flag
	It can be the carry produced after operation or the borrow in the case of subtraction.


# Don't Care(X)

Three bits are undefined.