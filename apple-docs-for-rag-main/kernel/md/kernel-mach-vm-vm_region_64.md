

- Kernel
- mach
- vm
-  vm_region_64 

Function

# vm_region_64

macOS 10.0+

``` source
kern_return_t vm_region_64(vm_map_read_t target_task, vm_address_t *address, vm_size_t *size, vm_region_flavor_t flavor, vm_region_info_t info, mach_msg_type_number_t *infoCnt, mach_port_t *object_name);
```

## See Also

### Regions

vm_region

vm_region_recurse

vm_region_recurse_64

vm_region_basic_info_data_64_t

vm_region_basic_info_data_t

vm_region_extended_info_data_t

vm_region_submap_info_data_64_t

vm_region_submap_info_data_t

vm_region_submap_short_info_data_64_t

vm_region_top_info_data_t

vm_page_info_basic_data_t

