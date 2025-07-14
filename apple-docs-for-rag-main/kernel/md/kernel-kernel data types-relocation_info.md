

- Kernel
- Kernel Data Types
-  relocation_info 

# relocation_info

macOS 10.8+

``` source
struct relocation_info {
    ...
};
```

## Topics

### Instance Properties

r_address

In `MH_OBJECT` files, an offset from the start of the section to the item containing the address requiring relocation.

r_extern

Indicates whether the `r_symbolnum` field is an index into the symbol table (1) or a section number (0).

r_length

Indicates the length of the item containing the address to be relocated.

r_pcrel

Indicates whether the item containing the address to be relocated is part of a CPU instruction that uses PC-relative addressing.

r_symbolnum

Indicates either an index into the symbol table (when the `r_extern` field is set to 1) or a section number (when the `r_extern` field is set to 0). As previously mentioned, sections are ordered from 1 to 255 in the order in which they appear in the `LC_SEGMENT` load commands. This field is set to `R_ABS` for relocation entries for absolute symbols, which need no relocation.

r_type

