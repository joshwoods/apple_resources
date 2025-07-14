

- Hypervisor
-  hv_vcpu_set_sys_reg(\_:\_:\_:) 

Function

# hv_vcpu_set_sys_reg(\_:\_:\_:)

Sets the value of a vCPU system register.

macOS 11.0+

``` source
func hv_vcpu_set_sys_reg(
    _ vcpu: hv_vcpu_t,
    _ reg: hv_sys_reg_t,
    _ value: UInt64
) -> hv_return_t
```

## Parameters 

`vcpu`  

The instance of the vCPU.

`reg`  

The ID of the system register.

`value`  

The new value of the register.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

Important

This function must be called by the owning thread.

## See Also

### System registers

func hv_vcpu_get_sys_reg(hv_vcpu_t, hv_sys_reg_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Gets the current value of a vCPU system register.

struct hv_sys_reg_t

The type of system registers.

