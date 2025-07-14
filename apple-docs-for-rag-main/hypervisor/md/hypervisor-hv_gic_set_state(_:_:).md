

- Hypervisor
-  hv_gic_set_state(\_:\_:) 

Function

# hv_gic_set_state(\_:\_:)

Sets the state of a generic interrupt controller (GIC) device.

macOS 15.0+

``` source
func hv_gic_set_state(
    _ gic_state_data: UnsafeRawPointer,
    _ gic_state_size: Int
) -> hv_return_t
```

## Parameters 

`gic_state_data`  

A pointer to the state buffer to use to set the GIC.

`gic_state_size`  

Size of GIC state buffer, in bytes.

## Return Value

HV_SUCCESS on success; otherwise, an error code.

## Discussion

Use this method to restore the state of a GIC. You can only restore a GIC’s state after creating a GIC device and vCPUs and before the vCPUs are running. Restore the rest of the virtual machine including GIC CPU registers with values that are compatible with the hv_gic_state_t.

In some cases this method can fail if a software update has changed the host in a way that would be incompatible with the previous format.

## See Also

### Getting and setting the GIC’s state

func hv_gic_state_create() -> hv_gic_state_t

Create a generic interrupt controller (GIC) state object.

func hv_gic_state_get_size(hv_gic_state_t, UnsafeMutablePointer&lt;Int>) -> hv_return_t

Gets the size of the buffer required for generic interrupt controller (GIC) state.

func hv_gic_state_get_data(hv_gic_state_t, UnsafeMutableRawPointer) -> hv_return_t

Gets the state data for generic interrupt controller (GIC).

typealias hv_gic_state_t

An alias for this value type’s equivalent Hypervisor generic interrupt controller (GIC) state’s reference type.

protocol OS_hv_gic_state

Methods that provide information on the hypervisor state.

