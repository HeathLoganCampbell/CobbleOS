# CobbleOS
A small OS

### Mindset
I just wanna try make a few basic things for fun, not for production use, not for some greater plan. just for fun

---
## Sat 26 2025
### Let's start.
First, we must start with hardware because you can't run software on thin air.
I kinda wanna go with a RISC-V since even in its name it promotes a reduced instruction set. Simple is good. Simple is a friend :)
So Longan nano seems promising. Cheap. Cheap is a friend.

### Learning the hardward
So the  Longan nano has a whole [website](https://wiki.sipeed.com/hardware/en/longan/Nano/Longan_nano.html) for him. 
It's a 32 bit computer, 32 KB of ram.
So I probably want the RV32I instruction set.
https://github.com/riscv/riscv-isa-manual/releases
ffs, this document is massive.
Time to use our best friend GPT to summarise

#### 🧩 Instruction Formats

Type	Meaning
R-type	Register-Register operations
I-type	Immediate operations, loads
S-type	Stores
B-type	Branches
U-type	Upper immediates
J-type	Jumps

<img width="819" alt="image" src="https://github.com/user-attachments/assets/32c36123-a035-4421-9c1f-1be634b7766c" />

Looks like a lot of effort, lets see if gpt and suggest a MORE reduce set

<img width="818" alt="image" src="https://github.com/user-attachments/assets/c2ce8e1a-e869-4c04-9205-07f1b9d6271c" />

I remember getting an assignment in UoA where we had to write a program to simulate [little computer 3](https://en.wikipedia.org/wiki/Little_Computer_3), which was a 16-bit computer. 
wonder if we could create that fictional PC but in real life.

#### Let's start with a simple program

```
.section .text
.global _start

_start:
    addi x1, x0, 5     # x1 = 5
    addi x2, x0, 10    # x2 = 10
    add  x3, x1, x2    # x3 = x1 + x2
    ebreak             # Stop execution
```

I guess it's simple to write an assembler to convert plain, clear English to machine code.

#### Abstraction is king
Software is all about abstraction.
Abstractions remove cognitive load in a few dimensions.
So sometimes It's fun to make your own abstractions from the ground up.

##### Level 1: Machine code.
I guess, I should learn how to write `hello world` in RISC Instruction set.



---
