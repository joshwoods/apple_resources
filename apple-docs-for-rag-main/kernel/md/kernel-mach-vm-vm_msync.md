

- Kernel
- mach
- vm
-  vm_msync 

Function

# vm_msync

macOS 10.0+

``` source
kern_return_t vm_msync(vm_map_t target_task, vm_address_t address, vm_size_t size, vm_sync_t sync_flags);
```

## See Also

### Configuration

vm_protect

vm_wire

mach_memory_info

vm_behavior_set

vm_machine_attribute

vm_purgable_control

vm_inherit

