## Number system 
- ### Binary
- ### Decimal 
- ### Hexadecimal
## Basics of x86 Architecture 

![CPU Architecture](/Assets/Pasted%20image%2020240428134947.png)

- CPU
	- ALU - A part of the CPU that carries out arithmetic or logical operations like `ADD`, `AND`,`OR` ,`NOT`
	- Control unit - Decode instructions into timing and control signal. 
	- Clock 
	- Registers - A type of memory which is close CPU and has faster transfer speeds compared to the normal memory. 
- Memory
- I/O devices 
- Bus 
	- Data bus - handle the transfer of data b/w CPU, memory and I/O. 
	- Control bus - Sync the actions b/w all the devices 
	- Address bus - Helps the hold the address of instruction and data transferred b/w the memory and CPU.

## Instruction Execution cycle 
#### Steps 
- Fetch the instruction 
- Decode the instruction and check the instructions.
- If operands are involved then fetch those operands from them the memory/register.
- Execute the instruction and update status flags
- store the result if required.

**Fetch Decode Execute** Procedure

## Reading from memory 
It's slower than reading from the register.
#### Steps 
- Place the address of the value youwnt to read on the address bus.
- Change the processor's RD pin (called assert ). More like setting it to READ mode.
- Waits one clock cycle for memory to respond 
- Copies the data from the data bus to the destination 

`Each` step takes place in `one clock cycle`.  `v/s` Register takes only `one clock cycle for the whole step`.

## Caching 
Main purpose - To reduce read/write time for memory.

In x86:
- Level - 1 cache is stored on the CPU.
- Level - 2 cache is stored outside and accessed by high speed data bus.
made by `static RAM` a type of RAM. it does not need to be refreshed constantly.
