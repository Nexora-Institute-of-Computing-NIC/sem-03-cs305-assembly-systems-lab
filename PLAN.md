# CS305 — Assembly & Systems Lab — PLAN

**Semester:** 3 · **Credits:** 2 · **Level:** Intermediate
**Theory:** 15 hrs · **Lab:** 30 hrs · **Tools:** x86-64 NASM or MIPS (MARS), gdb, objdump, ltrace, strace

## Syllabus

### Unit 1 — Assembly Fundamentals (8 lectures)
1. Why learn assembly — performance, debugging, security
2. CPU registers — general purpose and special
3. Instruction format — opcode, operands
4. Addressing modes
5. Load/store semantics
6. Data sizes — byte, word, dword, qword
7. Assembler, linker, loader
8. Compiling C to assembly — `gcc -S`

### Unit 2 — Instructions and Control Flow (7 lectures)
1. Arithmetic instructions — add, sub, imul, idiv
2. Logical and shift instructions
3. Comparisons — cmp, test
4. Conditional jumps
5. Loops and labels
6. Function calls — `call`, `ret`
7. The stack — push, pop, frame pointer

### Unit 3 — System Calls and Linux Interface (8 lectures)
1. User mode vs kernel mode revisited
2. The `syscall` instruction (x86-64) and `syscall` numbers
3. File operations — open, read, write, close
4. Process operations — fork, exec, exit
5. Signals — handling basics
6. Memory mapping — mmap and munmap
7. `strace` and `ltrace` — trace what the program does
8. Writing a "hello world" in raw assembly

### Unit 4 — Debugging and Reverse Engineering (7 lectures)
1. `gdb` basics — breakpoints, stepping, inspecting registers
2. Reading disassembly with `objdump`
3. Recognising loops, conditionals, and function prologues
4. Calling conventions — System V AMD64 ABI
5. Stack frames and unwinding
6. Buffer overflows — pattern recognition
7. Reverse-engineering a small binary

## Practical Labs (15)

1. Set up NASM, MARS, and the build toolchain
2. Print "Hello, world!" using Linux syscalls
3. Arithmetic in assembly — add, subtract, multiply
4. Implement a loop — sum of first N integers
5. Implement a conditional — max of two integers
6. Function calls — factorial implemented with `call`/`ret`
7. Recursion in assembly — Fibonacci
8. String processing — count characters in a string
9. Read input with the `read` syscall
10. Write output with the `write` syscall
11. File copy in assembly — open, read, write, close
12. Inspect a C binary with `objdump` — annotate instructions
13. Debug a crash with `gdb` — inspect registers and stack
14. Compare C and assembly — compile `gcc -S` and diff with your own
15. Trigger and observe a buffer overflow in a vulnerable program

## Assignments

1. Assembly instruction set — annotate a disassembled binary
2. Control flow — implement five small programs in assembly
3. System calls — implement file copy using only syscalls
4. Debugging report — analyse a crash with `gdb`
5. Reverse engineering — write up what a mystery binary does
