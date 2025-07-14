

- Kernel
- mach
- vm
-  vm_mapped_pages_info 

Function

# vm_mapped_pages_info

macOS 10.0+

``` source
kern_return_t vm_mapped_pages_info(vm_map_read_t task, page_address_array_t *pages, mach_msg_type_number_t *pagesCnt);
```

## See Also

### Memory Mapping

vm_map

vm_map_64

vm_map_exec_lockdown

vm_map_page_query

vm_remap

mach_make_memory_entry

mach_make_memory_entry_64

mach_memory_entry_access_tracking

mach_memory_entry_ownership

mach_memory_entry_purgable_control

