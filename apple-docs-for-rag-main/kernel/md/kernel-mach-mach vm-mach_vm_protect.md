

- Kernel
- mach
- Mach VM
-  mach_vm_protect 

Function

# mach_vm_protect

macOS 10.4+

``` source
kern_return_t mach_vm_protect(vm_map_t target_task, mach_vm_address_t address, mach_vm_size_t size, boolean_t set_maximum, vm_prot_t new_protection);
```

## See Also

### Configuration

mach_vm_wire

mach_vm_inherit

mach_vm_machine_attribute

mach_vm_msync

mach_vm_purgable_control

mach_vm_behavior_set

mach_vm_page_info

mach_vm_page_query

mach_vm_page_range_query

mach_vm_round_page_overflow

