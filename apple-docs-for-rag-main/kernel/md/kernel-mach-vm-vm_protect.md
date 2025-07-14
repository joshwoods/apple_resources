

- Kernel
- mach
- vm
-  vm_protect 

Function

# vm_protect

macOS 10.0+

``` source
kern_return_t vm_protect(vm_map_t target_task, vm_address_t address, vm_size_t size, boolean_t set_maximum, vm_prot_t new_protection);
```

## See Also

### Configuration

vm_wire

mach_memory_info

vm_behavior_set

vm_machine_attribute

vm_purgable_control

vm_inherit

vm_msync

