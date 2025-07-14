

- Hypervisor
-  hv_vcpu_set_reg(\_:\_:\_:) 

Function

# hv_vcpu_set_reg(\_:\_:\_:)

Sets the value of a vCPU register.

macOS 11.0+

``` source
func hv_vcpu_set_reg(
    _ vcpu: hv_vcpu_t,
    _ reg: hv_reg_t,
    _ value: UInt64
) -> hv_return_t
```

## Parameters 

`vcpu`  

The vCPU instance.

`reg`  

The ID of the general register.

`value`  

The new value of the register.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

Important

This function must be called by the owning thread.

## See Also

### General registers

func hv_vcpu_get_reg(hv_vcpu_t, hv_reg_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Gets the current value of a vCPU register.

struct hv_reg_t

The type that defines general registers.

