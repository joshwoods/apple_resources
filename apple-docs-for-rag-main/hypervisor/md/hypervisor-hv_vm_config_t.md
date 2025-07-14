

- Hypervisor
-  hv_vm_config_t 

Type Alias

# hv_vm_config_t

The type that defines a virtual-machine configuration.

macOS

``` source
typealias hv_vm_config_t = any OS_hv_vm_config
```

## See Also

### Virtual machine management

func hv_vm_config_create() -> hv_vm_config_t

Creates a virtual machine configuration object.

func hv_vm_create(hv_vm_options_t) -> hv_return_t

Creates a VM instance for the current process.

func hv_vm_destroy() -> hv_return_t

Destroys the VM instance associated with the current process.

protocol OS_hv_vm_config

Creates a virtual machine configuration object.

