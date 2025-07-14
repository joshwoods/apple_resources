

- Kernel
- mach-o
- dylib_command
-  cmd 

Instance Property

# cmd

Common to all load command structures. For this structure, set to either `LC_LOAD_DYLIB`, `LC_LOAD_WEAK_DYLIB`, or `LC_ID_DYLIB`.

macOS 10.6+

``` source
uint32_t cmd;
```

