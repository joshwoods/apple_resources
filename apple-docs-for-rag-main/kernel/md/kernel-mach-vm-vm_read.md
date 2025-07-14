

- Kernel
- mach
- vm
-  vm_read 

Function

# vm_read

macOS 10.0+

``` source
kern_return_t vm_read(vm_map_read_t target_task, vm_address_t address, vm_size_t size, vm_offset_t *data, mach_msg_type_number_t *dataCnt);
```

## See Also

### Reads and Writes

vm_read_list

vm_read_overwrite

vm_write

