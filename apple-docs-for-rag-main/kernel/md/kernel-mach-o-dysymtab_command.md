

- Kernel
- mach-o
-  dysymtab_command 

# dysymtab_command

macOS 10.6+

``` source
struct dysymtab_command {
    ...
};
```

## Topics

### Instance Properties

cmd

Common to all load command structures. For this structure, set to `LC_DYSYMTAB`.

cmdsize

extrefsymoff

An integer indicating the byte offset from the start of the file to the external reference table data.

extreloff

An integer indicating the byte offset from the start of the file to the external relocation table data.

iextdefsym

ilocalsym

indirectsymoff

iundefsym

locreloff

modtaboff

nextdefsym

nextrefsyms

nextrel

nindirectsyms

nlocalsym

nlocrel

nmodtab

ntoc

nundefsym

tocoff

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

dylib_table_of_contents

dylinker_command

