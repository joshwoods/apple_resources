

- Kernel
- mach
- vm
-  mach_make_memory_entry_64 

Function

# mach_make_memory_entry_64

macOS 10.0+

``` source
kern_return_t mach_make_memory_entry_64(vm_map_t target_task, memory_object_size_t *size, memory_object_offset_t offset, vm_prot_t permission, mach_port_t *object_handle, mem_entry_name_port_t parent_entry);
```

## See Also

### Memory Mapping

vm_map

vm_map_64

vm_map_exec_lockdown

vm_map_page_query

vm_mapped_pages_info

vm_remap

mach_make_memory_entry

mach_memory_entry_access_tracking

mach_memory_entry_ownership

mach_memory_entry_purgable_control

