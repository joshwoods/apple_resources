

- Hypervisor
-  hv_capability_t 

Type Alias

# hv_capability_t

The type of system capabilities.

macOS

``` source
typealias hv_capability_t = UInt64
```

## Topics

### Capabilities

var HV_CAP_VCPUMAX: Int

A value that indicates the maximum number of available vCPUs.

var HV_CAP_ADDRSPACEMAX: Int

A value that indicates the maximum number of available address spaces.

## See Also

### Virtual machine management

func hv_vm_create(hv_vm_options_t) -> hv_return_t

Creates a VM instance for the current process.

func hv_vm_destroy() -> hv_return_t

Destroys the VM instance associated with the current process.

func hv_capability(hv_capability_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Gets the value of capabilities of the system.

typealias hv_vm_options_t

Options you use when creating a virtual machine.

