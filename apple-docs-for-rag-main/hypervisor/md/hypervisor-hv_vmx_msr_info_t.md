

- Hypervisor
-  hv_vmx_msr_info_t 

Type Alias

# hv_vmx_msr_info_t

The type that describes Move to Status Register (MSR) information fields.

macOS

``` source
typealias hv_vmx_msr_info_t = UInt64
```

## See Also

### Capabilities

func hv_vmx_read_capability(hv_vmx_capability_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns, by reference, the VMX virtualization capabilities of the host processor.

func hv_vmx_get_msr_info(hv_vmx_msr_info_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns information about guest MSR configuration.

struct hv_vmx_capability_t

The type that describes Virtual Machine Extensions (VMX) capability fields.

VMX Capabilities

An enumeration that represents the available VMX capabilities.

MSR Information Fields

The type that describes Machine Specific Register (MSR) fields.

