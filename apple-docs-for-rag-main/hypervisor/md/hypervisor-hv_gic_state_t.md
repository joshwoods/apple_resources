

- Hypervisor
-  hv_gic_state_t 

Type Alias

# hv_gic_state_t

An alias for this value type’s equivalent Hypervisor generic interrupt controller (GIC) state’s reference type.

macOS

``` source
typealias hv_gic_state_t = any OS_hv_gic_state
```

## See Also

### Getting and setting the GIC’s state

func hv_gic_state_create() -> hv_gic_state_t

Create a generic interrupt controller (GIC) state object.

func hv_gic_set_state(UnsafeRawPointer, Int) -> hv_return_t

Sets the state of a generic interrupt controller (GIC) device.

func hv_gic_state_get_size(hv_gic_state_t, UnsafeMutablePointer&lt;Int>) -> hv_return_t

Gets the size of the buffer required for generic interrupt controller (GIC) state.

func hv_gic_state_get_data(hv_gic_state_t, UnsafeMutableRawPointer) -> hv_return_t

Gets the state data for generic interrupt controller (GIC).

protocol OS_hv_gic_state

Methods that provide information on the hypervisor state.

