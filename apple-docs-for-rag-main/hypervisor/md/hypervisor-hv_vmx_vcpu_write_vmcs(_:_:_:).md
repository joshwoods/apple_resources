

- Hypervisor
-  hv_vmx_vcpu_write_vmcs(\_:\_:\_:) 

Function

# hv_vmx_vcpu_write_vmcs(\_:\_:\_:)

Sets the value of a virtual machine control structure (VMCS) field of a vCPU.

macOS 10.10+

``` source
func hv_vmx_vcpu_write_vmcs(
    _ vcpu: hv_vcpuid_t,
    _ field: UInt32,
    _ value: UInt64
) -> hv_return_t
```

## Parameters 

`vcpu`  

The ID of the vCPU.

`field`  

The ID of the VMCS field. For a list of possible values, see `Virtual Machine Control Structure (VMCS) Field IDs`.

`value`  

The new value for `field` in the VMCS.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

Important

This function must be called by the owning thread.

## See Also

### Field management

Virtual Machine Control Structure (VMCS) Field IDs

Fields you can read or change using the Hypervisor framework’s read and write functions.

func hv_vmx_vcpu_read_vmcs(hv_vcpuid_t, UInt32, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns, by reference, the current value of a virtual machine control structure (VMCS) field of a vCPU.

func hv_vmx_vcpu_get_cap_write_vmcs(hv_vcpuid_t, UInt32, UnsafeMutablePointer&lt;UInt64>, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns the allowed_0 and allowed_1 masks for a VMCS field of a vCPU.

func hv_vmx_vcpu_set_apic_address(hv_vcpuid_t, hv_gpaddr_t) -> hv_return_t

Sets the address of the guest Advanced Programmable Interrupt Controller (APIC) for a vCPU in the guest physical address space of the VM.

Virtual Machine control structure (VMCS) Field IDs

Identify the fields of the virtual machine control structure.

