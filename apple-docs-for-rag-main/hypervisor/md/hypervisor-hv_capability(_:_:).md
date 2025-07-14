

- Hypervisor
-  hv_capability(\_:\_:) 

Function

# hv_capability(\_:\_:)

Gets the value of capabilities of the system.

macOS 10.15+

``` source
func hv_capability(
    _ capability: hv_capability_t,
    _ value: UnsafeMutablePointer
) -> hv_return_t
```

## Parameters 

`capability`  

The capability to request.

`value`  

The value for `capability`, on output.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

Intel-based Mac only.

## See Also

### Virtual machine management

func hv_vm_create(hv_vm_options_t) -> hv_return_t

Creates a VM instance for the current process.

func hv_vm_destroy() -> hv_return_t

Destroys the VM instance associated with the current process.

typealias hv_vm_options_t

Options you use when creating a virtual machine.

typealias hv_capability_t

The type of system capabilities.

