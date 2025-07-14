

- Kernel
- mach
- vm
-  vm_behavior_set 

Function

# vm_behavior_set

macOS 10.0+

``` source
kern_return_t vm_behavior_set(vm_map_t target_task, vm_address_t address, vm_size_t size, vm_behavior_t new_behavior);
```

## See Also

### Configuration

vm_protect

vm_wire

mach_memory_info

vm_machine_attribute

vm_purgable_control

vm_inherit

vm_msync

