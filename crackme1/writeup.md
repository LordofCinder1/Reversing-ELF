# <Crackme Name>

## Objective
Identify the flag through static analysis.

## Analysis

### Flag Generation
the encoded values for the flag are stored in `local_78`.

`memset()` sets the `0x41`(`'A'`) to the memory location of `local_98` for `0x1b` or 27 bytes

the `for loop` initializes the `local_78[0x1b]` to 0 first and it increments by 1 as long as it's less than 27

the values for each element of `local_78` will be added to the assigned value for `local_98` which is `0x41` 

after the loop, `local_98` contains the decoded characters and `puts()` displays it 


## Results
- Flag: `flag{not_that_kind_of_elf}`

## Tools
- Ghidra