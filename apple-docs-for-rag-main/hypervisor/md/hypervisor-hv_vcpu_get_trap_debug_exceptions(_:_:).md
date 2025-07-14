

- Hypervisor
-  hv_vcpu_get_trap_debug_exceptions(\_:\_:) 

Function

# hv_vcpu_get_trap_debug_exceptions(\_:\_:)

Gets whether debug exceptions exit the guest.

macOS 11.0+

``` source
func hv_vcpu_get_trap_debug_exceptions(
    _ vcpu: hv_vcpu_t,
    _ value: UnsafeMutablePointer
) -> hv_return_t
```

## Parameters 

`vcpu`  

The instance of the vCPU.

`value`  

Indicates whether debug exceptions in the guest trap to the host on output.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

The equivalent system register is `MDCR_EL2.TDE`.

Important

This function must be called by the owning thread.

## See Also

### Trap configuration

func hv_vcpu_set_trap_debug_exceptions(hv_vcpu_t, Bool) -> hv_return_t

Sets whether debug exceptions exit the guest.

func hv_vcpu_get_trap_debug_reg_accesses(hv_vcpu_t, UnsafeMutablePointer&lt;Bool>) -> hv_return_t

Gets whether debug-register accesses exit the guest.

func hv_vcpu_set_trap_debug_reg_accesses(hv_vcpu_t, Bool) -> hv_return_t

Sets whether debug-register accesses exit the guest.

