

- Kernel
- mach
- Mach VM
-  mach_vm_map 

Function

# mach_vm_map

macOS 10.4+

``` source
kern_return_t mach_vm_map(vm_map_t target_task, mach_vm_address_t *address, mach_vm_size_t size, mach_vm_offset_t mask, int flags, mem_entry_name_port_t object, memory_object_offset_t offset, boolean_t copy, vm_prot_t cur_protection, vm_prot_t max_protection, vm_inherit_t inheritance);
```

## See Also

### Memory Mapping

mach_vm_remap

