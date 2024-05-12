# Assembler & Simulator
- Based on a subset of RV32I (RISC-V 32 bit integer) instruction set.

## Assembler
- The assembler reads the assembly program as an input text file (stdin) and generates the binary (if there are no errors) as an output text file (stdout). If there are errors, the assembler generates the error notifications along with the line on which the error was encountered as an output text file (stdout).

## Simulator
- The input for the simulator is the binary file converted by the assembler. The simulator, after the execution of every instruction, prints the register values in any chosen file. The simulator will print the memory stats after the execution of the mentioned Virtual Halt instruction. 

# Problem
- Most of the assemblers I found online did not support most of the instructions I wanted them to. Furthermore, in my journey of computer graphics and building a game engine, I felt the need to make the assembler myself from scratch.
- The simulator is a complementary program to my assembler which provided fundamental information about the program and its execution essential for programming as well as debugging.

# How to use?
- Assembler\
`python3 Assembler.py <*.asm> <*.bin>` or `make asm`
- Simulator\
`python3 Simulator.py <*.bin> <output>` or `make sim`
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
