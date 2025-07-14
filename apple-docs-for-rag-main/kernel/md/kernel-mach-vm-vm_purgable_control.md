

- Kernel
- mach
- vm
-  vm_purgable_control 

Function

# vm_purgable_control

macOS 10.4+

``` source
kern_return_t vm_purgable_control(vm_map_t target_task, vm_address_t address, vm_purgable_t control, int *state);
```

## See Also

### Configuration

vm_protect

vm_wire

mach_memory_info

vm_behavior_set

vm_machine_attribute

vm_inherit

vm_msync

