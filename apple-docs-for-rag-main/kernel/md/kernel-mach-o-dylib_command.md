

- Kernel
- mach-o
-  dylib_command 

# dylib_command

macOS 10.6+

``` source
struct dylib_command {
    ...
};
```

## Topics

### Instance Properties

cmd

Common to all load command structures. For this structure, set to either `LC_LOAD_DYLIB`, `LC_LOAD_WEAK_DYLIB`, or `LC_ID_DYLIB`.

cmdsize

dylib

## See Also

### Dynamic Library Support

dyld_info_command

dyld_kernel_image_info_array_t

dyld_uuid_info_32

dyld_uuid_info_64

dyld_uuid_info_64_v2

dylib

dylib_module

dylib_module_64

dylib_reference

dylib_table_of_contents

dylinker_command

dysymtab_command

