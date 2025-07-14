

- Hypervisor
-  hv_vmx_get_msr_info(\_:\_:) 

Function

# hv_vmx_get_msr_info(\_:\_:)

Returns information about guest MSR configuration.

macOS 11.0+

``` source
func hv_vmx_get_msr_info(
    _ field: hv_vmx_msr_info_t,
    _ value: UnsafeMutablePointer
) -> hv_return_t
```

## Parameters 

`field`  

The ID of the MSR to examine.

`value`  

A pointer to the info field value written by Hypervisor on a successful operation.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Mentioned in 

Extending vCPU Capabilities Using Model-Specific Registers

## See Also

### Capabilities

func hv_vmx_read_capability(hv_vmx_capability_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns, by reference, the VMX virtualization capabilities of the host processor.

struct hv_vmx_capability_t

The type that describes Virtual Machine Extensions (VMX) capability fields.

VMX Capabilities

An enumeration that represents the available VMX capabilities.

typealias hv_vmx_msr_info_t

The type that describes Move to Status Register (MSR) information fields.

MSR Information Fields

The type that describes Machine Specific Register (MSR) fields.

