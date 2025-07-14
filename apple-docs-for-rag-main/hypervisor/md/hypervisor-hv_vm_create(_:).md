

- Hypervisor
-  hv_vm_create(\_:) 

Function

# hv_vm_create(\_:)

Creates a VM instance for the current process.

macOS 10.10+

``` source
func hv_vm_create(_ flags: hv_vm_options_t) -> hv_return_t
```

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

Intel-based Mac computers have different parameters:

`flags`  
Reserved. Pass HV_VM_DEFAULT to this argument.

## See Also

### Virtual machine management

func hv_vm_config_create() -> hv_vm_config_t

Creates a virtual machine configuration object.

func hv_vm_destroy() -> hv_return_t

Destroys the VM instance associated with the current process.

protocol OS_hv_vm_config

Creates a virtual machine configuration object.

typealias hv_vm_config_t

The type that defines a virtual-machine configuration.

