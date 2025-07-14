

- Kernel
- Kernel Data Types
- scattered_relocation_info
-  r_value 

Instance Property

# r_value

The address of the relocatable expression for the item in the file that needs to be updated if the address is changed. For relocatable expressions with the difference of two section addresses, the address from which to subtract (in mathematical terms, the minuend) is contained in the first relocation entry and the address to subtract (the subtrahend) is contained in the second relocation entry.

macOS 10.8+

``` source
int32_t r_value;
```

