

- Kernel
- mach
- vm
-  vm_write 

Function

# vm_write

macOS 10.0+

``` source
kern_return_t vm_write(vm_map_t target_task, vm_address_t address, vm_offset_t data, mach_msg_type_number_t dataCnt);
```

## See Also

### Reads and Writes

vm_read

vm_read_list

vm_read_overwrite

