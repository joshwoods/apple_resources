

- Kernel
- mach
- vm
-  vm_inherit 

Function

# vm_inherit

macOS 10.0+

``` source
kern_return_t vm_inherit(vm_map_t target_task, vm_address_t address, vm_size_t size, vm_inherit_t new_inheritance);
```

## See Also

### Configuration

vm_protect

vm_wire

mach_memory_info

vm_behavior_set

vm_machine_attribute

vm_purgable_control

vm_msync

