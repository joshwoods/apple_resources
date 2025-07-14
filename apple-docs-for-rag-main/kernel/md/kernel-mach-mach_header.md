

- Kernel
- mach
-  mach_header 

# mach_header

macOS 10.6+

``` source
struct mach_header {
    ...
};
```

## Topics

### Instance Properties

cpusubtype

cputype

filetype

flags

magic

An integer containing a value identifying this file as a 32-bit Mach-O file. Use the constant `MH_MAGIC` if the file is intended for use on a CPU with the same endianness as the computer on which the compiler is running. The constant `MH_CIGAM` can be used when the byte ordering scheme of the target machine is the reverse of the host CPU.

ncmds

sizeofcmds

## See Also

### Support

mach_atm_subaid_t

mach_core_details

mach_core_fileheader

mach_header_64

mach_bridge_regwrite_timestamp_func_t

