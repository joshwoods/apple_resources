

- Kernel
- mach
- vm
-  vm_allocate_cpm 

Function

# vm_allocate_cpm

macOS 10.0+

``` source
kern_return_t vm_allocate_cpm(host_priv_t host_priv, vm_map_t task, vm_address_t *address, vm_size_t size, int flags);
```

## See Also

### Creation and Destruction

vm_allocate

vm_deallocate

vm_copy

mach_vm_copy

