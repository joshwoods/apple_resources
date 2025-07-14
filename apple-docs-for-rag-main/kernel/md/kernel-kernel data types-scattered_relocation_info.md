

- Kernel
- Kernel Data Types
-  scattered_relocation_info 

# scattered_relocation_info

macOS 10.8+

``` source
struct scattered_relocation_info {
    ...
};
```

## Topics

### Instance Properties

r_address

r_length

r_pcrel

Indicates whether the item containing the address to be relocated is part of a CPU instruction that uses PC-relative addressing.

r_scattered

If this bit is 0, this structure is actually a relocation_info structure.

r_type

Indicates the type of relocation to be performed. Possible values for this field are shared between this structure and the `relocation_info` data structure; see the description of the `r_type` field in the relocation_info data structure for more details.

r_value

The address of the relocatable expression for the item in the file that needs to be updated if the address is changed. For relocatable expressions with the difference of two section addresses, the address from which to subtract (in mathematical terms, the minuend) is contained in the first relocation entry and the address to subtract (the subtrahend) is contained in the second relocation entry.

