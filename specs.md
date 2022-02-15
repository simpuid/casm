# Specs

## Registers
32 bit registers named from `r0` to `r31`

## Instructions

`set <destination register> <32-bit intermediate value>`

`add <destination register> <operand register> <operand register>`

`mul <destination register> <operand register> <operand register>`

`beq <operand register> <operand register> <jump location>`

`jmp <jump location>`

## Marking
`<mark name>:` will mark the next instruction.

Used in `beq` and `jmp` instructions

## Factorial

```asm
set r0 0 
set r1 1

set r2 5 # Calculating 5 factorial

set r3 1 # Holds the result
set r4 1 # Loop iterator

my_loop:
beq r4 r2 my_finish
add r4 r4 r1
mul r3 r3 r4
jmp my_loop
my_finish:
```

