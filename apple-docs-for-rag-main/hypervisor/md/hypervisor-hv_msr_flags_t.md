

- Hypervisor
-  hv_msr_flags_t 

Type Alias

# hv_msr_flags_t

The type representing the native Model-Specific Register (MSR) permissions.

macOS

``` source
typealias hv_msr_flags_t = UInt32
```

## Discussion

This type represents the native MSR permissions for `hv_vm_enable_managed_msr()`. The MSR Permissions enumeration describes the available permission values.

## See Also

### Model-Specific Registers

Extending vCPU Capabilities Using Model-Specific Registers

Configure specific client performance monitoring and enable other vCPU capabilities using Model-Specific Registers.

func hv_vcpu_read_msr(hv_vcpuid_t, UInt32, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns, by reference, the current value of a Model-Specific Register (MSR) of a vCPU.

func hv_vcpu_write_msr(hv_vcpuid_t, UInt32, UInt64) -> hv_return_t

Sets the value of a Model-Specific Register (MSR) of a vCPU.

func hv_vcpu_enable_native_msr(hv_vcpuid_t, UInt32, Bool) -> hv_return_t

Enables or disables a Model-Specific Register (MSR) that the VM uses natively.

func hv_vcpu_set_msr_access(hv_vcpuid_t, UInt32, hv_msr_flags_t) -> hv_return_t

Controls the guest access of a managed Model-Specific Register (MSR).

func hv_vcpu_enable_managed_msr(hv_vcpuid_t, UInt32, Bool) -> hv_return_t

Enables the guest access of a managed Model-Specific Register (MSR).

Model-Specific Registers

MSR Permissions

An enumeration that describes possible Model-Specific Register (MSR) permisssions.

