

- Hypervisor
-  hv_vmx_read_capability(\_:\_:) 

Function

# hv_vmx_read_capability(\_:\_:)

Returns, by reference, the VMX virtualization capabilities of the host processor.

macOS 10.10+

``` source
func hv_vmx_read_capability(
    _ field: hv_vmx_capability_t,
    _ value: UnsafeMutablePointer
) -> hv_return_t
```

## Parameters 

`field`  

The capability of the host processor to return. For a list of field IDs, see hv_vmx_capability_t.

`value`  

The value of the capability `field`, on output. For a list of possible values, see `VMX Capability Field Values`.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

Important

This function must be called by the owning thread.

## See Also

### Capabilities

func hv_vmx_get_msr_info(hv_vmx_msr_info_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns information about guest MSR configuration.

struct hv_vmx_capability_t

The type that describes Virtual Machine Extensions (VMX) capability fields.

VMX Capabilities

An enumeration that represents the available VMX capabilities.

typealias hv_vmx_msr_info_t

The type that describes Move to Status Register (MSR) information fields.

MSR Information Fields

The type that describes Machine Specific Register (MSR) fields.

