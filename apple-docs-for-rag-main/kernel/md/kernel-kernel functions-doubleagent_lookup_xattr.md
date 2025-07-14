

- Kernel
- Kernel Functions
-  doubleagent_lookup_xattr 

Function

# doubleagent_lookup_xattr

macOS 15.0+

``` source
kern_return_t doubleagent_lookup_xattr(mach_port_t server, mach_port_t file_port, int64_t file_size, xattrname name, int *err, uint64_t *value_offset, uint64_t *value_length);
```

