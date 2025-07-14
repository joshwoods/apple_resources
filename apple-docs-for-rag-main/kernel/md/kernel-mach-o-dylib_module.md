

- Kernel
- mach-o
-  dylib_module 

# dylib_module

macOS 10.6+

``` source
struct dylib_module {
    ...
};
```

## Topics

### Instance Properties

iextdefsym

iextrel

The index into the external relocation table of the first entry provided by this module.

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

The number of external reference entries provided by this module.

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

dylib_module_64

dylib_reference

dylib_table_of_contents

dylinker_command

dysymtab_command

