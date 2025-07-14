

- Kernel
- mach-o
-  dylib_table_of_contents 

# dylib_table_of_contents

macOS 10.6+

``` source
struct dylib_table_of_contents {
    ...
};
```

## Topics

### Instance Properties

module_index

symbol_index

An index into the symbol table indicating the defined external symbol to which this entry refers.

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

dylib_reference

dylinker_command

dysymtab_command

