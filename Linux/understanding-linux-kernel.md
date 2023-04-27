## Chapter 1

![](/Users/zhourui/Desktop/Screen%20Shot%202023-04-25%20at%2010.41.45%20PM.png)

Kernel manages the process, and each process is represented by a process descriptor, which saves following info

- PC and stack pointer (SP) registers

- The general purpose registers

- Floating point registers

- The processor control registers containg info about CPU state

- The memory management registers to keep track of RAM accessed 



### Semaphores

Semaphores is simply just a counter to count up and down based on number of accessed threaded

- A counter (integer)

- List of waiting processes

- down() and up()



For example, we could set counter to 1. If every a thread enters CR (crtitical region), down() to 0. All other threads check the counter and wait in the list.



### Spin Locks

In order to resolve the efficiency issue from Semaphores (use time short). 

- No process list

- 
