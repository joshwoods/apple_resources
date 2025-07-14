

- Kernel
- mach
- vm
-  vm_machine_attribute 

Function

# vm_machine_attribute

macOS 10.0+

``` source
kern_return_t vm_machine_attribute(vm_map_t target_task, vm_address_t address, vm_size_t size, vm_machine_attribute_t attribute, vm_machine_attribute_val_t *value);
```

## See Also

### Configuration

vm_protect

vm_wire

mach_memory_info

vm_behavior_set

vm_purgable_control

vm_inherit

vm_msync

