

- Kernel
- Kernel Data Types
- relocation_info
-  r_pcrel 

Instance Property

# r_pcrel

Indicates whether the item containing the address to be relocated is part of a CPU instruction that uses PC-relative addressing.

macOS 10.8+

``` source
uint32_t r_pcrel:1;
```

## Discussion

For addresses contained in PC-relative instructions, the CPU adds the address of the instruction to the address contained in the instruction.

