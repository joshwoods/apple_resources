

- Hypervisor
-  hv_gic_state_get_size(\_:\_:) 

Function

# hv_gic_state_get_size(\_:\_:)

Gets the size of the buffer required for generic interrupt controller (GIC) state.

macOS 15.0+

``` source
func hv_gic_state_get_size(
    _ state: hv_gic_state_t,
    _ gic_state_size: UnsafeMutablePointer
) -> hv_return_t
```

## Parameters 

`state`  

The GIC state object.

`gic_state_size`  

The pointer to GIC data size, that the framework writes to upon success.

## Return Value

HV_SUCCESS on success; otherwise, an error code.

## See Also

### Getting and setting the GIC’s state

func hv_gic_state_create() -> hv_gic_state_t

Create a generic interrupt controller (GIC) state object.

func hv_gic_set_state(UnsafeRawPointer, Int) -> hv_return_t

Sets the state of a generic interrupt controller (GIC) device.

func hv_gic_state_get_data(hv_gic_state_t, UnsafeMutableRawPointer) -> hv_return_t

Gets the state data for generic interrupt controller (GIC).

typealias hv_gic_state_t

An alias for this value type’s equivalent Hypervisor generic interrupt controller (GIC) state’s reference type.

protocol OS_hv_gic_state

Methods that provide information on the hypervisor state.

