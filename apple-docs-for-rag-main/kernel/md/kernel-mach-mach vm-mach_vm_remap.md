

- Kernel
- mach
- Mach VM
-  mach_vm_remap 

Function

# mach_vm_remap

macOS 10.4+

``` source
kern_return_t mach_vm_remap(vm_map_t target_task, mach_vm_address_t *target_address, mach_vm_size_t size, mach_vm_offset_t mask, int flags, vm_map_t src_task, mach_vm_address_t src_address, boolean_t copy, vm_prot_t *cur_protection, vm_prot_t *max_protection, vm_inherit_t inheritance);
```

## See Also

### Memory Mapping

mach_vm_map

