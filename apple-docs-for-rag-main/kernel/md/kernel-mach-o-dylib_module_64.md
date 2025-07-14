

- Kernel
- mach-o
-  dylib_module_64 

# dylib_module_64

macOS 10.6+

``` source
struct dylib_module_64 {
    ...
};
```

## Topics

### Instance Properties

iextdefsym

iextrel

iinit_iterm

ilocalsym

irefsym

module_name

nextdefsym

nextrel

ninit_nterm

Contains both the number of pointers in the module initialization (the low 16 bits) and the number of pointers in the module termination section (the high 16 bits) for this module.

nlocalsym

nrefsym

objc_module_info_addr

objc_module_info_size

## See Also

### Dynamic Library Support

dyld_info_command

dyld_kernel_image_info_array_t

dyld_uuid_info_32

dyld_uuid_info_64

dyld_uuid_info_64_v2

dylib

dylib_command

dylib_module

dylib_reference

dylib_table_of_contents

dylinker_command

dysymtab_command

