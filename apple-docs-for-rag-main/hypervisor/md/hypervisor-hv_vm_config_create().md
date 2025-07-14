

- Hypervisor
-  hv_vm_config_create() 

Function

# hv_vm_config_create()

Creates a virtual machine configuration object.

macOS 13.0+

``` source
func hv_vm_config_create() -> hv_vm_config_t
```

## Return Value

A new virtual-machine configuration object. Release this object with `os_release` when no longer used.

## See Also

### Virtual machine management

func hv_vm_create(hv_vm_options_t) -> hv_return_t

Creates a VM instance for the current process.

func hv_vm_destroy() -> hv_return_t

Destroys the VM instance associated with the current process.

protocol OS_hv_vm_config

Creates a virtual machine configuration object.

typealias hv_vm_config_t

The type that defines a virtual-machine configuration.

