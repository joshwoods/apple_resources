

- Kernel
- mach
- Mach VM
-  mach_vm_inherit 

Function

# mach_vm_inherit

macOS 10.4+

``` source
kern_return_t mach_vm_inherit(vm_map_t target_task, mach_vm_address_t address, mach_vm_size_t size, vm_inherit_t new_inheritance);
```

## See Also

### Configuration

mach_vm_protect

mach_vm_wire

mach_vm_machine_attribute

mach_vm_msync

mach_vm_purgable_control

mach_vm_behavior_set

mach_vm_page_info

mach_vm_page_query

mach_vm_page_range_query

mach_vm_round_page_overflow

