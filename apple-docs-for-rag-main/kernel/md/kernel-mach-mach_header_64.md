

- Kernel
- mach
-  mach_header_64 

# mach_header_64

macOS 10.6+

``` source
struct mach_header_64 {
    ...
};
```

## Topics

### Instance Properties

cpusubtype

An integer specifying the exact model of the CPU. To run on all PowerPC processors supported by the macOS kernel, this should be set to `CPU_SUBTYPE_POWERPC_ALL`.

cputype

filetype

flags

An integer containing a set of bit flags that indicate the state of certain optional features of the Mach-O file format. These are the masks you can use to manipulate this field:

magic

An integer containing a value identifying this file as a 64-bit Mach-O file. Use the constant `MH_MAGIC_64` if the file is intended for use on a CPU with the same endianness as the computer on which the compiler is running. The constant `MH_CIGAM_64` can be used when the byte ordering scheme of the target machine is the reverse of the host CPU.

ncmds

reserved

sizeofcmds

## See Also

### Support

mach_atm_subaid_t

mach_core_details

mach_core_fileheader

mach_header

mach_bridge_regwrite_timestamp_func_t

