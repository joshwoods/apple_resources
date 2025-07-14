

- Hypervisor
-  hv_vmx_vcpu_write_shadow_vmcs(\_:\_:\_:) 

Function

# hv_vmx_vcpu_write_shadow_vmcs(\_:\_:\_:)

Set the value of a shadow VMCS field of a vCPU.

macOS 10.15+

``` source
func hv_vmx_vcpu_write_shadow_vmcs(
    _ vcpu: hv_vcpuid_t,
    _ field: UInt32,
    _ value: UInt64
) -> hv_return_t
```

## Parameters 

`vcpu`  

The vCPU ID.

`field`  

The ID of the shadow VMCS field to write.

`value`  

The value of the shadow VMCS field to write.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

Important

This function must be called by the owning thread.

## See Also

### Shadow fields

func hv_vmx_vcpu_read_shadow_vmcs(hv_vcpuid_t, UInt32, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns the current value of a shadow VMCS field of a vCPU.

func hv_vmx_vcpu_set_shadow_access(hv_vcpuid_t, UInt32, hv_shadow_flags_t) -> hv_return_t

Set the access permissions of a shadow VMCS field of a vCPU.

typealias hv_shadow_flags_t

Shadow VMCS permissions for the set shadow access function.

Shadow Permissions

Permissions that define access to the shadow VMCS fields.

