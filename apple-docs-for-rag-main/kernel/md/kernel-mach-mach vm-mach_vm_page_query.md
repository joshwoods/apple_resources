

- Kernel
- mach
- Mach VM
-  mach_vm_page_query 

Function

# mach_vm_page_query

macOS 10.4+

``` source
kern_return_t mach_vm_page_query(vm_map_read_t target_map, mach_vm_offset_t offset, integer_t *disposition, integer_t *ref_count);
```

## See Also

### Configuration

mach_vm_protect

mach_vm_wire

mach_vm_inherit

mach_vm_machine_attribute

mach_vm_msync

mach_vm_purgable_control

mach_vm_behavior_set

mach_vm_page_info

mach_vm_page_range_query

mach_vm_round_page_overflow

