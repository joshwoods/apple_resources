

- Hypervisor
-  hv_vcpu_get_vtimer_mask(\_:\_:) 

Function

# hv_vcpu_get_vtimer_mask(\_:\_:)

Gets the virtual timer mask.

macOS 11.0+

``` source
func hv_vcpu_get_vtimer_mask(
    _ vcpu: hv_vcpu_t,
    _ vtimer_is_masked: UnsafeMutablePointer
) -> hv_return_t
```

## Parameters 

`vcpu`  

The ID of the vCPU instance.

`vtimer_is_masked`  

The value of the mask.

## Return Value

HV_SUCCESS if the operation was successful, otherwise an error code specified in hv_return_t.

## See Also

### Timer functions

func hv_vcpu_set_vtimer_mask(hv_vcpu_t, Bool) -> hv_return_t

Sets or clears the virtual timer mask.

func hv_vcpu_get_vtimer_offset(hv_vcpu_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Returns the vTimer offset for the vCPU ID you specify.

func hv_vcpu_set_vtimer_offset(hv_vcpu_t, UInt64) -> hv_return_t

Sets the vTimer offset to a value that you provide.

