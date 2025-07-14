

- Kernel
- mach
- vm
-  vm_wire 

Function

# vm_wire

macOS 10.0+

``` source
kern_return_t vm_wire(host_priv_t host_priv, vm_map_t task, vm_address_t address, vm_size_t size, vm_prot_t desired_access);
```

## See Also

### Configuration

vm_protect

mach_memory_info

vm_behavior_set

vm_machine_attribute

vm_purgable_control

vm_inherit

vm_msync

