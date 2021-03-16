# FIT1008 W1PartBNotes

[toc]



### 0. introduction to MIPS and its architecture

Note:

### Part 1

- von Neumann architecture

![image-20210308203153463](https://tva1.sinaimg.cn/large/008eGmZEgy1gocrvkxb0mj30ng0aojs8.jpg)

instructions and data must be loaded into the CPU before being processed.

CPU runs machine code written in machine language, which is always 32 bits

- machine code & machine language
- what's words
- what's assembly language?
  - support comments, labels, variable names
  - Human-readable
  - easily convert to machine language
- how to convert high-level language into machine code

- RISC(Reduced Instruction Set Computer)

  - same length, 4 bytes which is 32 bits or a word
  - of similar simple complexity
  - 1 clock cycle
  - easily decoded and executed by computer hardware

- x86 CISC(Complex Instruction Set Computer)

  - instruction vary in length, complexity and execution time
  - usually for complex work, like graph game

- many different types of microprocessor architecture

  

### Part 2

- MIPS Architecture
- the main basics components
  - 32 bits general-purpose registers: memory
  - ALU: performs computations
  - Special-purpose register
    - PC
    - HI, LO
    - IR
    - MAR/MRR/MWR(Memory Address/Read/Write Register)
- General Purpose Registers(GPRs)
  - prefixed with $
  - can't name them yourself

- arithemetic instructions

  - sub, addi, xor, div

- special purpose registers(HI & LO)

  - if multiplying two 32 bites numbers might require 64 bits 
  - like 5/3 will get the integer 1 and the remainder 2
  - LO contains the integer
  - HI contains the remaindar

- Instruction Register(IR)

  - it stores the instruciton currently being execude
  - like sub, addi, xor
  - The IR isn't visible for programer

- Program Counter(PC)

  - tells the computer where is it up to, act like a bookmark
  - it holds the memory address of the machine instruction currently being executed

- MIPS Instruciton Execution

  - Fetch next instruction from memory and placed in IR
  - decode instruction in the IR to determine type
  - execute instruction
  - continue the above steps from the beginning

  

### Part 3 mips memory

- mips is a load-store architecture, and it only stored results and computations in register
- programs and thier data live in main memory instead of CPU chip
- memory is divided into segments from address A to address B
  - text
  - data(static/heap)
  - stack
- memory address in mips are 32 bits long, so the total potential address space is 4Gb. The range is  32 bits  of  zero to $$2^{32}-1 $$. 
- why memory is divided into segment? Because you don't know the sequence of binary numer's representation. It could be a number or ASCII charater.
  - so program variables have types
- use a **load word(lw)** intruction's process
  - ![image-20210308214808977](https://tva1.sinaimg.cn/large/008eGmZEgy1gocu2xkgqij31b40nsjvv.jpg)

- use a **store word(sw)** into main memory
  - ![image-20210308215003304](https://tva1.sinaimg.cn/large/008eGmZEgy1gocu4wn7asj31c40lo782.jpg)

- memory architecture
  - ![image-20210308215431550](https://tva1.sinaimg.cn/large/008eGmZEgy1gocu9ksm5qj31bm0k8q7g.jpg)
- Text segment
  - starts at 0x0040000000, if the memory address smaller than it are reserved for the OS
  - when loading , PC will points it 
- Data segment
  - divided into 2 parts
  - first for static 
  - second for dynamic
- Heap segment
  - it locates at the end, after all the static data
  - all python objects and thier instance varibales go here
  - grows downwards
  - Empty at the start of program execution
- Stack segment
  - grows upwards
  - it's used for the temporary storage of function information, local variables, saved register values.





Q:

- what's the difference between memory and register in CPU, since both of them can store things. 
- what's the difference betweeen machine code and machine language?
- why IR is invisible for programer? 
- when to use text or data assembly detectives?



## Changelog

- 2021-03-08 2h init