

- Hypervisor
-  hv_gic_config_set_distributor_base(\_:\_:) 

Function

# hv_gic_config_set_distributor_base(\_:\_:)

Sets the generic interrupt controller (GIC) distributor region’s base address.

macOS 15.0+

``` source
func hv_gic_config_set_distributor_base(
    _ config: hv_gic_config_t,
    _ distributor_base_address: hv_ipa_t
) -> hv_return_t
```

## Parameters 

`config`  

The GIC configuration object.

`distributor_base_address`  

The guest’s physical address for the distributor.

## Return Value

A new GIC configuration object.

## Discussion

Guest physical address for the distributor base aligned to the byte value returned by hv_gic_get_distributor_base_alignment(_:).

Release this object with os_release when it’s no longer needed.

## See Also

### Setting the GIC device configuration

func hv_gic_config_create() -> hv_gic_config_t

Creates a generic interrupt controller (GIC) configuration object.

func hv_gic_config_set_redistributor_base(hv_gic_config_t, hv_ipa_t) -> hv_return_t

Sets the generic interrupt controller (GIC) redistributor region base address.

func hv_gic_get_redistributor_base(hv_vcpu_t, UnsafeMutablePointer&lt;hv_ipa_t>) -> hv_return_t

Gets the redistributor base guest physical address for the given vCPU.

func hv_gic_config_set_msi_region_base(hv_gic_config_t, hv_ipa_t) -> hv_return_t

Sets the generic interrupt controllers message signaled interrupts (MSIs) region base address.

func hv_gic_config_set_msi_interrupt_range(hv_gic_config_t, UInt32, UInt32) -> hv_return_t

Sets the range of message signaled interrupts (MSIs) the generic interrupt controller supports.

protocol OS_hv_gic_config

Methods that provide information on the state of a generic interrupt controller.

typealias hv_gic_config_t

An alias for this value type’s equivalent Hypervisor generic interrupt controller (GIC) configuration’s reference type.

