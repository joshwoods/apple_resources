

- Hypervisor
-  hv_vcpu_read_register(\_:\_:\_:) 

Function

# hv_vcpu_read_register(\_:\_:\_:)

Returns, by reference, the current value of an architectural x86 register of a vCPU.

macOS 10.10+

``` source
func hv_vcpu_read_register(
    _ vcpu: hv_vcpuid_t,
    _ reg: hv_x86_reg_t,
    _ value: UnsafeMutablePointer
) -> hv_return_t
```

## Parameters 

`vcpu`  

The instance of the vCPU.

`reg`  

The ID of the register. For possible values, see hv_x86_reg_t.

`value`  

The value of the register `reg`, on output.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## Discussion

Important

This function must be called by the owning thread.

## See Also

### CPU Registers

func hv_vcpu_write_register(hv_vcpuid_t, hv_x86_reg_t, UInt64) -> hv_return_t

Sets the value of an architectural x86 register of a vCPU.

struct hv_x86_reg_t

The type that defines x86 architectural registers.

