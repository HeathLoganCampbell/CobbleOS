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





---
