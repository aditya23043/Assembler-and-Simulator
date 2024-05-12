# Assembler & Simulator
- Based on a subset of RV32I (RISC-V 32 bit integer) instruction set.

## Assembler
- The assembler reads the assembly program as an input text file (stdin) and generates the binary (if there are no errors) as an output text file (stdout). If there are errors, the assembler generates the error notifications along with the line on which the error was encountered as an output text file (stdout).

## Simulator
- The input for the simulator is the binary file converted by the assembler. The simulator, after the execution of every instruction, prints the register values in any chosen file. The simulator will print the memory stats after the execution of the mentioned Virtual Halt instruction. 

# How to use?
- Assembler\
`python3 Assembler.py <*.asm> <*.bin>`
- Simulator\
`python3 Simulator.py <*.bin> <output>`
- Here \<output\> is a text file which contains all register and memory stats during and after the program execution

# Supported Instructions
- add
- sub
- slt
- sltu
- xor
- sll
- srl
- or
- and
- lw
- addi
- sltiu
- jalr
- sw
- beq
- bne
- bge
- bgeu
- blt
- bltu
- auipc
- lui
- jal
- mul
- rst
- halt
- rvrs
