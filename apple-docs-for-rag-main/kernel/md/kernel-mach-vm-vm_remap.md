

- Kernel
- mach
- vm
-  vm_remap 

Function

# vm_remap

macOS 10.0+

``` source
kern_return_t vm_remap(vm_map_t target_task, vm_address_t *target_address, vm_size_t size, vm_address_t mask, int flags, vm_map_t src_task, vm_address_t src_address, boolean_t copy, vm_prot_t *cur_protection, vm_prot_t *max_protection, vm_inherit_t inheritance);
```

## See Also

### Memory Mapping

vm_map

vm_map_64

vm_map_exec_lockdown

vm_map_page_query

vm_mapped_pages_info

mach_make_memory_entry

mach_make_memory_entry_64

mach_memory_entry_access_tracking

mach_memory_entry_ownership

mach_memory_entry_purgable_control

