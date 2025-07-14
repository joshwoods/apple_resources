

- Hypervisor
-  hv_tsc_clock() 

Function

# hv_tsc_clock()

Returns the value of an abstract clock.

macOS 11.0+

``` source
func hv_tsc_clock() -> UInt64
```

## Return Value

A 64-bit unsigned integer that represents the current clock value.

## Discussion

The abstract clock ticks at the same rate as the host TSC, offset by an implementation-dependent constant. The clock value increases monotonically.

## See Also

### Time-stamp counter functions

func hv_vcpu_set_tsc_relative(hv_vcpuid_t, Int64) -> hv_return_t

Sets the offset of the guest timestamp-counter (TSC) relative to the Hypervisor’s TSC clock.

