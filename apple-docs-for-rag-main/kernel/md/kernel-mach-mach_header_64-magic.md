

- Kernel
- mach
- mach_header_64
-  magic 

Instance Property

# magic

An integer containing a value identifying this file as a 64-bit Mach-O file. Use the constant `MH_MAGIC_64` if the file is intended for use on a CPU with the same endianness as the computer on which the compiler is running. The constant `MH_CIGAM_64` can be used when the byte ordering scheme of the target machine is the reverse of the host CPU.

macOS 10.6+

``` source
uint32_t magic;
```

