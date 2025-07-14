

- Kernel
- mach
- Mach VM
-  mach_vm_page_range_query 

Function

# mach_vm_page_range_query

macOS 10.13+

``` source
kern_return_t mach_vm_page_range_query(vm_map_read_t target_map, mach_vm_offset_t address, mach_vm_size_t size, mach_vm_address_t dispositions, mach_vm_size_t *dispositions_count);
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

mach_vm_page_query

mach_vm_round_page_overflow

