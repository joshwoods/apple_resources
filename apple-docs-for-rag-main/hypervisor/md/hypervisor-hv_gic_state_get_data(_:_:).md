

- Hypervisor
-  hv_gic_state_get_data(\_:\_:) 

Function

# hv_gic_state_get_data(\_:\_:)

Gets the state data for generic interrupt controller (GIC).

macOS 15.0+

``` source
func hv_gic_state_get_data(
    _ state: hv_gic_state_t,
    _ gic_state_data: UnsafeMutableRawPointer
) -> hv_return_t
```

## Parameters 

`state`  

The GIC state object.

`gic_state_data`  

Pointer to GIC state buffer that the framework writes to upon success.

## Return Value

HV_SUCCESS on success; otherwise, an error code.

## Discussion

The function returns an opaque data buffer that contains the complete serialized state of the device, except for the GIC CPU registers. You can write the data to a file and is stable. It’s also versioned which allows the framework to detect incompatibilities when it restores the state. The size of this GIC state buffer must be at least as large as the size returned by hv_gic_state_get_size(_:_:).

You can read GIC CPU system registers separately, and save them to be able to restore the CPU state for the virtual machine.

## See Also

### Getting and setting the GIC’s state

func hv_gic_state_create() -> hv_gic_state_t

Create a generic interrupt controller (GIC) state object.

func hv_gic_set_state(UnsafeRawPointer, Int) -> hv_return_t

Sets the state of a generic interrupt controller (GIC) device.

func hv_gic_state_get_size(hv_gic_state_t, UnsafeMutablePointer&lt;Int>) -> hv_return_t

Gets the size of the buffer required for generic interrupt controller (GIC) state.

typealias hv_gic_state_t

An alias for this value type’s equivalent Hypervisor generic interrupt controller (GIC) state’s reference type.

protocol OS_hv_gic_state

Methods that provide information on the hypervisor state.

