

- Kernel
- mach-o
-  dylib_reference 

# dylib_reference

macOS 10.6+

``` source
struct dylib_reference {
    ...
};
```

## Topics

### Instance Properties

flags

isym

An index into the symbol table for the symbol being referenced.

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

dylib_module_64

dylib_table_of_contents

dylinker_command

dysymtab_command

