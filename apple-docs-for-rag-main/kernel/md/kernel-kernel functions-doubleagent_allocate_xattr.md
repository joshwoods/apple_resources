

- Kernel
- Kernel Functions
-  doubleagent_allocate_xattr 

Function

# doubleagent_allocate_xattr

macOS 15.0+

``` source
kern_return_t doubleagent_allocate_xattr(mach_port_t server, mach_port_t file_port, int64_t file_size, xattrname name, uint64_t size, uint32_t options, int *err, uint64_t *value_offset);
```

