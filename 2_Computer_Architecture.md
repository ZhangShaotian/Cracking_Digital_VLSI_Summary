# Chapter 2: Computer Architecture
## 51. Difference between RISC and CISC architectures
RISC: Reduced Instruction Set Computer  
CISC: Complex Instruction Set Computer  
- RISC has less number of instructions and they are simpler(fixed length, less addressing mode)
- RISC has smaller instructions, while CISC has a more complex hardware to decode or handle the complex instructions. Therefore, RISC's emphasis is more on software.
- Since CICS has complex hardware, it requires smaller software codes and hence less RAM to store programming instructions.
- RISC aims to improve performance by reducing number of cycles of instruction whereas CISC attmpts to improve performance by minizing number of instructions per program.

Addressing Mode:  
- Immediate Addressing: The operand is in instruction itself
- Register Addressing: The operand is located in CPU register.
- Direct Addressing: The memory address of the operand is in the instruction.
- Indirect Addressing: The memory address of the memory address of the operand is specified in the instruction.
## 52. Difference between Von-Neumann and Harvard Architecture.
In Von-Neumann Arch, there is a single memory that can hold both data and instruction. Typically, this would mean that there is a signle bus between CPU to memory that accesses both data and instruction. The Harvard Arch is the opposite. 
## 53. Little Endian and Big Endian formats
- Little Endian: LSB is stored in smallest address.
- Big Endian: MSB is stored in smallest address.  
It's important in low level programming.