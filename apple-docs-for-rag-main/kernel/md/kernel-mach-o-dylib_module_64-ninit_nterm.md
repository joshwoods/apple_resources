

- Kernel
- mach-o
- dylib_module_64
-  ninit_nterm 

Instance Property

# ninit_nterm

Contains both the number of pointers in the module initialization (the low 16 bits) and the number of pointers in the module termination section (the high 16 bits) for this module.

macOS 10.6+

``` source
uint32_t ninit_nterm;
```

