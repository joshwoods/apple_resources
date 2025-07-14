

- Kernel
- Kernel Data Types
-  fat_arch 

# fat_arch

Describes the location within the binary of an object file targeted at a single architecture. Declared in `/usr/include/mach-o/fat.h`.

macOS 10.8+

``` source
struct fat_arch {
    ...
};
```

## Discussion

An array of `fat_arch` data structures appears directly after the fat_header data structure of a binary that contains object files for multiple architectures.

Regardless of the content this data structure describes, all its fields are stored in big-endian byte order.

## Topics

### Fields

cpusubtype

An enumeration value of type `cpu_subtype_t`. Specifies the specific member of the CPU family on which this entry may be used or a constant specifying all members.

offset

Offset to the beginning of the data for this CPU.

size

Size of the data for this CPU.

align

The power of 2 alignment for the offset of the object file for the architecture specified in `cputype` within the binary. This is required to ensure that, if this binary is changed, the contents it retains are correctly aligned for virtual memory paging and other uses.

### Instance Properties

cputype

