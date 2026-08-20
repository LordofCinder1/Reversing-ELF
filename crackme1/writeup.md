# <Crackme Name>

## Objective
Identify the flag through static analysis.

## Analysis

### Flag Generation
the charcters to the flag are already displayed in `local_78` elements already.

`memset()` sets the `0x41`(`'A'`) to the memory location of `local_98` for `0x1b` or 27 bytes

the `for loop` initializes the `local_78[0x1b]` to 0 first and it increments by 1 as long as it's less than 27

getting the values for each element of `local_78` will be added to the assigned value for `local_98` which is `0x41` will generate the flag


## Results
- Flag: `flag{not_that_kind_of_elf}`

## Tools
- Ghidra