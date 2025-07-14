

- Kernel
- mach
- Mach VM
-  mach_vm_wire 

Function

# mach_vm_wire

macOS 10.4+

``` source
kern_return_t mach_vm_wire(host_priv_t host_priv, vm_map_t task, mach_vm_address_t address, mach_vm_size_t size, vm_prot_t desired_access);
```

## See Also

### Configuration

mach_vm_protect

mach_vm_inherit

mach_vm_machine_attribute

mach_vm_msync

mach_vm_purgable_control

mach_vm_behavior_set

mach_vm_page_info

mach_vm_page_query

mach_vm_page_range_query

mach_vm_round_page_overflow

