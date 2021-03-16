[TOC]



# FIT1008 Solo Prac2(in lab)

Five coding practices

first one

- defining and printing strings in mips
- The line number of every MIPS instruction and the purpose of the instruction. 
- The name of any label. 
- Line number of any assembly directive and the purpose of the directive. 
- Name of any global variable. 
- Name of any general-purpose register used.



```
# Author: Jieying Li
# Print a line using mips
# Begin coding here
    .data
prompt: .asciiz "I am really enjoying MIPS"
nl:		.asciiz "\n"

    .text
    # print the statment
    addi $v0, $0, 4
    la $a0, prompt
    syscall

    # print new line as python's print method
    la $a0, nl 
    addi $v0, $0, 4 
    syscall         

    # Exit
    addi $v0, $0, 10
    syscall
```





second, writing 

Run the first one code and answer the following questions.

1: What does PC refer to? What is the initial value of Register PC, see how PC changes as you step through the program. Is there a pattern in the change of value? 
A: 

- PC refer to program counter which holds the address of the instruction being executed at the current time.

-  The initial value of PC is 0xFFF0, and then increasing by 4 bites through each instruction.

  





2: Has every MIPS instruction been assembled into a single machine code instruction? Explain why/why not with examples
A: Not all of them have been assembled into machine code, like assembler directives won't be translate into machine code. And the rest of the mips will convert into machine code.





3: What does the data segment hold and represent?  NOTE: Maybe it helps to click the check-box ASCII.

A: The data segment holds the address of  "I am really enjoying MIPS" and "\n". And its representation is like this picture: ![image-20210310155538613](/Users/leigitwing/Library/Application Support/typora-user-images/image-20210310155538613.png)





Third,

input two numbers and print the quotient and remainder of them.





Forth,

more maths, pythagorean 





```mips
lw $t0, m
lw $t1, n 
mult $t0, $t0
mflo $t0  # m^2
mult $t1, $t1
mflo $t1  # n^2
sub $t2, $t0, $t1
sw $t2, a

# print the value of a
lw $a0, a
addi $v0, $0, 1 
syscall
```




fivth

reads any two integers and determines if the first one is a multiple of the second one. 

It will need if branch to check if reminder is zero.



## FIT1008 Workshop





## FIT1008 interview prac







 

## FIT1008 Tute 2

simple, convert print statement in python to mips instructions





## Changelog

- 2021-03-09 add interview prac

- 2021-03-08 init