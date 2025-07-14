

- Hypervisor
-  hv_shadow_flags_t 

Type Alias

# hv_shadow_flags_t

Shadow VMCS permissions for the set shadow access function.

macOS

``` source
typealias hv_shadow_flags_t = UInt64
```

## See Also

### Shadow fields

func hv_vmx_vcpu_read_shadow_vmcs(hv_vcpuid_t, UInt32, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns the current value of a shadow VMCS field of a vCPU.

func hv_vmx_vcpu_set_shadow_access(hv_vcpuid_t, UInt32, hv_shadow_flags_t) -> hv_return_t

Set the access permissions of a shadow VMCS field of a vCPU.

func hv_vmx_vcpu_write_shadow_vmcs(hv_vcpuid_t, UInt32, UInt64) -> hv_return_t

Set the value of a shadow VMCS field of a vCPU.

Shadow Permissions

Permissions that define access to the shadow VMCS fields.

