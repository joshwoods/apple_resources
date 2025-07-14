

- Kernel
- Kernel Data Types
- fat_header
-  magic 

Instance Property

# magic

An integer containing the value `0xCAFEBABE` in big-endian byte order format. On a big-endian host CPU, this can be validated using the constant `FAT_MAGIC`; on a little-endian host CPU, it can be validated using the constant `FAT_CIGAM`.

macOS 10.8+

``` source
uint32_t magic;
```

