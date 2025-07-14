

- Hypervisor
-  OS_hv_vm_config 

Protocol

# OS_hv_vm_config

Creates a virtual machine configuration object.

macOS

``` source
protocol OS_hv_vm_config : NSObjectProtocol
```

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Virtual machine management

func hv_vm_config_create() -> hv_vm_config_t

Creates a virtual machine configuration object.

func hv_vm_create(hv_vm_options_t) -> hv_return_t

Creates a VM instance for the current process.

func hv_vm_destroy() -> hv_return_t

Destroys the VM instance associated with the current process.

typealias hv_vm_config_t

The type that defines a virtual-machine configuration.

