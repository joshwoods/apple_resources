

- Kernel
- mach
- vm
-  mach_memory_info 

Function

# mach_memory_info

macOS 10.11+

``` source
kern_return_t mach_memory_info(mach_port_t host, mach_zone_name_array_t *names, mach_msg_type_number_t *namesCnt, mach_zone_info_array_t *info, mach_msg_type_number_t *infoCnt, mach_memory_info_array_t *memory_info, mach_msg_type_number_t *memory_infoCnt);
```

## See Also

### Configuration

vm_protect

vm_wire

vm_behavior_set

vm_machine_attribute

vm_purgable_control

vm_inherit

vm_msync

