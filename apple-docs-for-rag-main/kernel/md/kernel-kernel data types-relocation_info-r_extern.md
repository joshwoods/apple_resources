

- Kernel
- Kernel Data Types
- relocation_info
-  r_extern 

Instance Property

# r_extern

Indicates whether the `r_symbolnum` field is an index into the symbol table (1) or a section number (0).

macOS 10.8+

``` source
uint32_t r_extern:1;
```

