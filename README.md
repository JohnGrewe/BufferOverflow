## Buffer Overflow
$sudosysctl-wkernel.randomize_va_space=0

$sudoln-sf/bin/zsh/bin/sh

gcc-DBUF_SIZE=100-m32-ostack-zexecstack-fno-stack-protectorstack.c

p $ebp: 0xffffce98
p &buffer: 0xffffce2c

![image](https://github.com/JohnGrewe/BufferOverflow/assets/112670893/c193cb23-5c08-47a9-9071-a2024976d402)


![image](https://github.com/JohnGrewe/BufferOverflow/assets/112670893/21b3b5b5-8ffa-4fca-b248-0d7ee31b8958)



I got unlucky with the random number guessing, put in like 50 inputs


This lab taught me about how buffer overflows, if not taken precaution against, can lead to 3rd parties gaining control of root users and being able to do whatever they want with them. Even though I got unlucky with my attack, there is only 400 guesses for L1 so if someone were to have the time, I could see this becoming an actual threat

I also learned on how to intercept hexes in code to be able to use the buffer overflow attack by debugging and making break points
