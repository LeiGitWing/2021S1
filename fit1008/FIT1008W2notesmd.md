## FIT1008W2notes

[toc]

## PartA: L04 Decisions

### outcome

- learn coditional control tranfer instructions
- learn comparison instructions
- how to use them to translate simple if-else
- faithful meaning

### notes

using j instruction to demenstrate `goto` statement in python.

faithful means load and store values 



comparison instruciton & branch insturction to represent control statement in python

- branch instruction

`beq $t0, $t1, foo # if t0 == t1 goto foo function`

`bne $to, $t2, foo # if t0 !=t1 goto foo function`

- comparison instruction 

![image-20210315112926691](https://tva1.sinaimg.cn/large/e6c9d24egy1gokfjbyfy5j21g20e6tb1.jpg)



putting it all together

![image-20210315112053827](https://tva1.sinaimg.cn/large/e6c9d24egy1gokfajxjucj21f60j4jwu.jpg)



### Q:

- when translating faitful, why we need to add $v0 to 1 again?

- why we need a signed offset? In which condition we will use it to allocate an address?

-   ✓What does pseudoinstructions mean?

  - They transform into several instructions. And we are not allowed to use them excepte for `la` instrucion.

  



## PartB: Decisons and Iterations

### Outcome

- more complex if-else statement
- translate for and while loop



[Tutorial 1 recording ver1 Passcode: fZX5WLFbNsh=

[Tutorial 1 recording ver2 Passcode: 7*NU6biky5hD



## PartC: Arrays in MIPS

This part has the biggest slides. 



## Tute Notes

- To understand how to implement decisions and loops in MIPS.
- arrays and how to implement them in mips



most of them are loops and arrays, not very much if-then



## Workshop Notes

There are three questions and i still confused about all of them. 

first one is a if-else, the second one is while loop, the third one is array





## Interview prac

Task 1: complex if-esle 

Task 2: for loop, if-else, array

Task 3: functional version of task 2

Task 4: bubble sort in mips



## Changelog



- 2021-03-14 init