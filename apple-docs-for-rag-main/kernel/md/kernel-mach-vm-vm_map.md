

- Kernel
- mach
- vm
-  vm_map 

Function

# vm_map

macOS 10.0+

``` source
kern_return_t vm_map(vm_map_t target_task, vm_address_t *address, vm_size_t size, vm_address_t mask, int flags, mem_entry_name_port_t object, vm_offset_t offset, boolean_t copy, vm_prot_t cur_protection, vm_prot_t max_protection, vm_inherit_t inheritance);
```

## See Also

### Memory Mapping

vm_map_64

vm_map_exec_lockdown

vm_map_page_query

vm_mapped_pages_info

vm_remap

mach_make_memory_entry

mach_make_memory_entry_64

mach_memory_entry_access_tracking

mach_memory_entry_ownership

mach_memory_entry_purgable_control

