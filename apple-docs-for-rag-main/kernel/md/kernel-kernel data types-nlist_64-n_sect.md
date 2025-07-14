

- Kernel
- Kernel Data Types
- nlist_64
-  n_sect 

Instance Property

# n_sect

An integer specifying the number of the section that this symbol can be found in, or `NO_SECT` if the symbol is not to be found in any section of this image. The sections are contiguously numbered across segments, starting from 1, according to the order they appear in the `LC_SEGMENT` load commands.

macOS 10.8+

``` source
uint8_t n_sect;
```

## See Also

### Fields

n_un

A union that holds an index into the string table, `n_strx`. To specify an empty string (`""`), set this value to 0.

n_type

A byte value consisting of data accessed using four bit masks:

n_desc

A 16-bit value providing additional information about the nature of this symbol. The reference flags can be accessed using the `REFERENCE_TYPE` mask (0xF) and are defined as follows:

