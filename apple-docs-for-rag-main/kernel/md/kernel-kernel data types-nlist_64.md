

- Kernel
- Kernel Data Types
-  nlist_64 

# nlist_64

Describes an entry in the symbol table for 64-bit architectures. Declared in `/usr/include/mach-o/nlist.h`.

macOS 10.8+

``` source
struct nlist_64 {
    ...
};
```

## Discussion

See discussion in nlist.

## Topics

### Fields

n_un

A union that holds an index into the string table, `n_strx`. To specify an empty string (`""`), set this value to 0.

n_type

A byte value consisting of data accessed using four bit masks:

n_sect

An integer specifying the number of the section that this symbol can be found in, or `NO_SECT` if the symbol is not to be found in any section of this image. The sections are contiguously numbered across segments, starting from 1, according to the order they appear in the `LC_SEGMENT` load commands.

n_desc

A 16-bit value providing additional information about the nature of this symbol. The reference flags can be accessed using the `REFERENCE_TYPE` mask (0xF) and are defined as follows:

### Instance Properties

n_value

