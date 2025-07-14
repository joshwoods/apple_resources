

- Hypervisor
-  hv_vcpu_write_msr(\_:\_:\_:) 

Function

# hv_vcpu_write_msr(\_:\_:\_:)

Sets the value of a Model-Specific Register (MSR) of a vCPU.

macOS 10.10+

``` source
func hv_vcpu_write_msr(
    _ vcpu: hv_vcpuid_t,
    _ msr: UInt32,
    _ value: UInt64
) -> hv_return_t
```

## Parameters 

`vcpu`  

The instance of the vCPU.

`msr`  

The ID of the MSR.

`value`  

The new value for `msr`.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

This function must be called by the owning thread.

## See Also

### Model-Specific Registers

Extending vCPU Capabilities Using Model-Specific Registers

Configure specific client performance monitoring and enable other vCPU capabilities using Model-Specific Registers.

func hv_vcpu_read_msr(hv_vcpuid_t, UInt32, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns, by reference, the current value of a Model-Specific Register (MSR) of a vCPU.

func hv_vcpu_enable_native_msr(hv_vcpuid_t, UInt32, Bool) -> hv_return_t

Enables or disables a Model-Specific Register (MSR) that the VM uses natively.

func hv_vcpu_set_msr_access(hv_vcpuid_t, UInt32, hv_msr_flags_t) -> hv_return_t

Controls the guest access of a managed Model-Specific Register (MSR).

func hv_vcpu_enable_managed_msr(hv_vcpuid_t, UInt32, Bool) -> hv_return_t

Enables the guest access of a managed Model-Specific Register (MSR).

typealias hv_msr_flags_t

The type representing the native Model-Specific Register (MSR) permissions.

Model-Specific Registers

MSR Permissions

An enumeration that describes possible Model-Specific Register (MSR) permisssions.

