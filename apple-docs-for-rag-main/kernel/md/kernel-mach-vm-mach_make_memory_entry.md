

- Kernel
- mach
- vm
-  mach_make_memory_entry 

Function

# mach_make_memory_entry

macOS 10.0+

``` source
kern_return_t mach_make_memory_entry(vm_map_t target_task, vm_size_t *size, vm_offset_t offset, vm_prot_t permission, mem_entry_name_port_t *object_handle, mem_entry_name_port_t parent_entry);
```

## See Also

### Memory Mapping

vm_map

vm_map_64

vm_map_exec_lockdown

vm_map_page_query

vm_mapped_pages_info

vm_remap

mach_make_memory_entry_64

mach_memory_entry_access_tracking

mach_memory_entry_ownership

mach_memory_entry_purgable_control

