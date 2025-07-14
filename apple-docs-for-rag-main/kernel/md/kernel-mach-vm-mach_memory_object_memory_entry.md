

- Kernel
- mach
- vm
-  mach_memory_object_memory_entry 

Function

# mach_memory_object_memory_entry

macOS 10.0+

``` source
kern_return_t mach_memory_object_memory_entry(host_t host, boolean_t internal, vm_size_t size, vm_prot_t permission, memory_object_t pager, mach_port_t *entry_handle);
```

## See Also

### Memory Objects

mach_memory_object_memory_entry_64

