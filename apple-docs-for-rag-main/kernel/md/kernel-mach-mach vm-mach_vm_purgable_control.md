

- Kernel
- mach
- Mach VM
-  mach_vm_purgable_control 

Function

# mach_vm_purgable_control

macOS 10.5+

``` source
kern_return_t mach_vm_purgable_control(vm_map_t target_task, mach_vm_address_t address, vm_purgable_t control, int *state);
```

## See Also

### Configuration

mach_vm_protect

mach_vm_wire

mach_vm_inherit

mach_vm_machine_attribute

mach_vm_msync

mach_vm_behavior_set

mach_vm_page_info

mach_vm_page_query

mach_vm_page_range_query

mach_vm_round_page_overflow

