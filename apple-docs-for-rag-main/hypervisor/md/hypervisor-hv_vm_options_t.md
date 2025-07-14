

- Hypervisor
-  hv_vm_options_t 

Type Alias

# hv_vm_options_t

Options you use when creating a virtual machine.

macOS

``` source
typealias hv_vm_options_t = UInt64
```

## Topics

### Options

var HV_VM_DEFAULT: Int

The default VM creation behavior.

## See Also

### Virtual machine management

func hv_vm_create(hv_vm_options_t) -> hv_return_t

Creates a VM instance for the current process.

func hv_vm_destroy() -> hv_return_t

Destroys the VM instance associated with the current process.

func hv_capability(hv_capability_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Gets the value of capabilities of the system.

typealias hv_capability_t

The type of system capabilities.

