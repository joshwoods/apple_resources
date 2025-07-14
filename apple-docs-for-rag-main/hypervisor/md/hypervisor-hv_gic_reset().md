

- Hypervisor
-  hv_gic_reset() 

Function

# hv_gic_reset()

Resets the generic interrupt controller (GIC) device.

macOS 15.0+

``` source
func hv_gic_reset() -> hv_return_t
```

## Return Value

HV_SUCCESS on success, an error code otherwise.

## Discussion

When you’re resetting the virtual machine, call this function to reset the GIC distributor, redistributor registers and the internal state of the device.

