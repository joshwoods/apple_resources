

- Hypervisor
-  hv_vcpu_set_vtimer_offset(\_:\_:) 

Function

# hv_vcpu_set_vtimer_offset(\_:\_:)

Sets the vTimer offset to a value that you provide.

macOS 11.0+

``` source
func hv_vcpu_set_vtimer_offset(
    _ vcpu: hv_vcpu_t,
    _ vtimer_offset: UInt64
) -> hv_return_t
```

## Parameters 

`vcpu`  

The ID of the vCPU instance.

`vtimer_offset`  

The new vTimer offset.

## Return Value

`0` on success, or an error code of the type hv_return_t.

## Discussion

This corresponds to the value of the `CNTVOFF_EL2` register.

## See Also

### Timer functions

func hv_vcpu_get_vtimer_mask(hv_vcpu_t, UnsafeMutablePointer&lt;Bool>) -> hv_return_t

Gets the virtual timer mask.

func hv_vcpu_set_vtimer_mask(hv_vcpu_t, Bool) -> hv_return_t

Sets or clears the virtual timer mask.

func hv_vcpu_get_vtimer_offset(hv_vcpu_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns the vTimer offset for the vCPU ID you specify.

