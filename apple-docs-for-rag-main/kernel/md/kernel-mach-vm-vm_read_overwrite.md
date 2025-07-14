

- Kernel
- mach
- vm
-  vm_read_overwrite 

Function

# vm_read_overwrite

macOS 10.0+

``` source
kern_return_t vm_read_overwrite(vm_map_read_t target_task, vm_address_t address, vm_size_t size, vm_address_t data, vm_size_t *outsize);
```

## See Also

### Reads and Writes

vm_read

vm_read_list

vm_write

