

- Kernel
- mach
- mach_header
-  magic 

Instance Property

# magic

An integer containing a value identifying this file as a 32-bit Mach-O file. Use the constant `MH_MAGIC` if the file is intended for use on a CPU with the same endianness as the computer on which the compiler is running. The constant `MH_CIGAM` can be used when the byte ordering scheme of the target machine is the reverse of the host CPU.

macOS 10.6+

``` source
uint32_t magic;
```

