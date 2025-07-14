

- Kernel
- mach
- vm
-  vm_map_page_query 

Function

# vm_map_page_query

macOS 10.0+

``` source
kern_return_t vm_map_page_query(vm_map_read_t target_map, vm_offset_t offset, integer_t *disposition, integer_t *ref_count);
```

## See Also

### Memory Mapping

vm_map

vm_map_64

vm_map_exec_lockdown

vm_mapped_pages_info

vm_remap

mach_make_memory_entry

mach_make_memory_entry_64

mach_memory_entry_access_tracking

mach_memory_entry_ownership

mach_memory_entry_purgable_control

