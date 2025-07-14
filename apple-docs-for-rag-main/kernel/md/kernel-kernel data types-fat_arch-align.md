

- Kernel
- Kernel Data Types
- fat_arch
-  align 

Instance Property

# align

The power of 2 alignment for the offset of the object file for the architecture specified in `cputype` within the binary. This is required to ensure that, if this binary is changed, the contents it retains are correctly aligned for virtual memory paging and other uses.

macOS 10.8+

``` source
uint32_t align;
```

## See Also

### Fields

cpusubtype

An enumeration value of type `cpu_subtype_t`. Specifies the specific member of the CPU family on which this entry may be used or a constant specifying all members.

offset

Offset to the beginning of the data for this CPU.

size

Size of the data for this CPU.

