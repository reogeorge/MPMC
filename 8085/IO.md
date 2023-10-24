The main signal related to Input output is IO/M signal

IO/M determines if a operation is on memory or on I/O
	If the signal is high, then the operation is on I/O, otherwise on memory

IO/M along with the status flags **S0,S1**  indicate the operation that is to be performed

| **IO/M** | **S1** | **S0** | **Machine Cycle**     |
|----------|--------|--------|-----------------------|
| 0        | 0      | 1      | Memory Write(MW)      |
| 0        | 1      | 0      | Memory Read(MR)       |
| 0        | 1      | 1      | Opcode Fetch(OF)      |
| 1        | 0      | 1      | I/O Write(IOW)        |
| 1        | 1      | 0      | I/O Read(IOR)         |
| 1        | 1      | 1      | Interrupt Acknowledge |

basically write, read, custom.

## Additional IO signals


**READ(RD)**
	Signals that the selected memory or I/O device is ready to be read from and the data bus is ready to transfer data


**Write(WR)**
	Signals that the memory/ IO is ready to be write whatever is in the data bus.


**Ready**
	Signals that the memory or IO is ready to be read written

[[8085 Intel|Back to timing and control]]