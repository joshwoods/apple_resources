

- Kernel
- mach
- vm
-  mach_memory_entry_ownership 

Function

# mach_memory_entry_ownership

macOS 10.15+

``` source
kern_return_t mach_memory_entry_ownership(mem_entry_name_port_t mem_entry, task_t owner, int ledger_tag, int ledger_flags);
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

mach_make_memory_entry_64

mach_memory_entry_access_tracking

mach_memory_entry_purgable_control

