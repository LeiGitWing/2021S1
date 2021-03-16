# FIT1008 W1PartCNotes

[toc]

TODO:

- [ ] PART 4 NOTES



## 0. Intro to assembly program

### Part 1

- Main components
- mips asssembly directives and how to use them in program

- label(define and use it)
  - ![image-20210308223427271](https://tva1.sinaimg.cn/large/008eGmZEgy1gocvf3vtxhj31fg0rgn3g.jpg)

- definition of assembler directives
- common type of assebler directives
  - switch mode
    - .data
    - .text
  - allocate space
    - .space N
    - .word w1[,w2, w3...]
    - .asciiz "string"



### Part 2 MIPS instructions

- basic kinds
  - ![image-20210308223745656](https://tva1.sinaimg.cn/large/008eGmZEgy1gocvijz4emj31aa0po0xe.jpg)
- integer
  - add
  - addi
  - sub
  - mult
  - div
- data movement instructions
  - move from HI: mfhi
  - move from LO: mflo
- load and store instructions
- Addressing Formats
  - ![image-20210308225135058](https://tva1.sinaimg.cn/large/008eGmZEgy1gocvwx7jqhj31ga0rmgqt.jpg) 





Q:

- When to use .text assembler directives?
  - [What is .word, .data and .text in assembly? - Stack Overflow](https://stackoverflow.com/questions/60403872/what-is-word-data-and-text-in-assembly) `.text` tells the assembler where the codes go, and the `.data` tells where the data should be stored, `.word` is like an array, creating some space in memory to hold data.
- what's the meaning of $0? Does it represent address in register?
  - just hold the content of zero. 
- what's the difference between switch mode and allocate space of assebler directives?
- what's the difference between add and addi?
- ![image-20210308224724908](https://tva1.sinaimg.cn/large/008eGmZEgy1gocvslbw6dj31fk0s2wmk.jpg)



### Part 3

Bitwise and shift

- Bitwise
  - AND&
  - OR|
  - exclusive OR^
  - Not-or ~( $t1 | $t2 )
- sneaky assebler tricks
  - pseudoinstructions

- shift
  - ![image-20210308225903003](https://tva1.sinaimg.cn/large/008eGmZEgy1gocw4pg7nrj31is0totii.jpg)





### Part 4

§ To learn how to use unconditional control transfer instructions

§ To learn the three different instruction formats



- label vs goto statement
- mips's goto -- control transfer instructions
- 





### Q:









## Changelog

- 2021-03-08 init