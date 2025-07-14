

- Kernel
- mach
- Mach VM
-  mach_vm_region 

Function

# mach_vm_region

macOS 10.4+

``` source
kern_return_t mach_vm_region(vm_map_read_t target_task, mach_vm_address_t *address, mach_vm_size_t *size, vm_region_flavor_t flavor, vm_region_info_t info, mach_msg_type_number_t *infoCnt, mach_port_t *object_name);
```

## See Also

### Regions

mach_vm_region_info

mach_vm_region_info_64

mach_vm_region_recurse

