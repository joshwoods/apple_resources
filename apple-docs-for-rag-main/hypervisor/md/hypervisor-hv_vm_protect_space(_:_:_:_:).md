

- Hypervisor
-  hv_vm_protect_space(\_:\_:\_:\_:) 

Function

# hv_vm_protect_space(\_:\_:\_:\_:)

Modifies the permissions of a region in a guest physical address space of the VM.

macOS 10.15+

``` source
func hv_vm_protect_space(
    _ asid: hv_vm_space_t,
    _ gpa: hv_gpaddr_t,
    _ size: Int,
    _ flags: hv_memory_flags_t
) -> hv_return_t
```

## Parameters 

`asid`  

The address space ID.

`gpa`  

The page aligned address in the guest physical address space.

`size`  

The size in bytes of the region to unmap.

`flags`  

The new `READ`, `WRITE` and `EXECUTE` permissions of the region.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## See Also

### Functions

func hv_sme_config_get_max_svl_bytes(UnsafeMutablePointer&lt;Int>) -> hv_return_t

func hv_vcpu_apic_ctrl(hv_vcpuid_t, hv_apic_ctrl_t) -> hv_return_t

func hv_vcpu_apic_get_state(hv_vcpuid_t, UnsafeMutablePointer&lt;hv_apic_state_ext_t>) -> hv_return_t

func hv_vcpu_apic_lsc_enter_imm32(hv_vcpuid_t, UInt64, UInt32, UInt16, UInt32, UnsafeMutablePointer&lt;UInt64>?, UInt32) -> hv_return_t

func hv_vcpu_apic_lsc_enter_r32(hv_vcpuid_t, Bool, UInt64, UInt32, UInt16, hv_x86_reg_t, UnsafeMutablePointer&lt;UInt64>?, UInt32) -> hv_return_t

func hv_vcpu_apic_lsc_invalidate(hv_vcpuid_t) -> hv_return_t

func hv_vcpu_apic_put_state(hv_vcpuid_t, UnsafePointer&lt;hv_apic_state_ext_t>) -> hv_return_t

func hv_vcpu_apic_read(hv_vcpuid_t, UInt32, UnsafeMutablePointer&lt;UInt32>) -> hv_return_t

func hv_vcpu_apic_trigger_lvt(hv_vcpuid_t, hv_apic_lvt_flavor_t) -> hv_return_t

func hv_vcpu_apic_write(hv_vcpuid_t, UInt32, UInt32, UnsafeMutablePointer&lt;Bool>) -> hv_return_t

func hv_vcpu_exit_apic_access_read(hv_vcpuid_t, UnsafeMutablePointer&lt;UInt32>) -> hv_return_t

func hv_vcpu_exit_info(hv_vcpuid_t, UnsafeMutablePointer&lt;hv_vm_exitinfo_t>) -> hv_return_t

func hv_vcpu_exit_init_ap(hv_vcpuid_t, UnsafeMutablePointer&lt;Bool>, UInt32) -> hv_return_t

func hv_vcpu_exit_inject_excp(hv_vcpuid_t, UnsafeMutablePointer&lt;UInt8>, UnsafeMutablePointer&lt;Bool>, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;Bool>) -> hv_return_t

func hv_vcpu_exit_ioapic_eoi(hv_vcpuid_t, UnsafeMutablePointer&lt;UInt8>) -> hv_return_t

