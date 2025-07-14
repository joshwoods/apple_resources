

- Kernel
- mach
- Mach VM
-  mach_vm_msync 

Function

# mach_vm_msync

macOS 10.4+

``` source
kern_return_t mach_vm_msync(vm_map_t target_task, mach_vm_address_t address, mach_vm_size_t size, vm_sync_t sync_flags);
```

## See Also

### Configuration

mach_vm_protect

mach_vm_wire

mach_vm_inherit

mach_vm_machine_attribute

mach_vm_purgable_control

mach_vm_behavior_set

mach_vm_page_info

mach_vm_page_query

mach_vm_page_range_query

mach_vm_round_page_overflow

