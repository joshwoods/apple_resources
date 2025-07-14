

- Hypervisor
-  hv_gic_config_set_msi_region_base(\_:\_:) 

Function

# hv_gic_config_set_msi_region_base(\_:\_:)

Sets the generic interrupt controllers message signaled interrupts (MSIs) region base address.

macOS 15.0+

``` source
func hv_gic_config_set_msi_region_base(
    _ config: hv_gic_config_t,
    _ msi_region_base_address: hv_ipa_t
) -> hv_return_t
```

## Parameters 

`config`  

A GIC configuration object.

`msi_region_base_address`  

The guest’s physical address for a MSI region.

## Return Value

HV_SUCCESS on success; otherwise, an error code.

## Discussion

Align the guest physical address for MSI region base to the byte value returned by hv_gic_get_msi_region_base_alignment(_:).

For MSI support, set the interrupt range with hv_gic_config_set_msi_interrupt_range(_:_:_:).

## See Also

### Setting the GIC device configuration

func hv_gic_config_create() -> hv_gic_config_t

Creates a generic interrupt controller (GIC) configuration object.

func hv_gic_config_set_distributor_base(hv_gic_config_t, hv_ipa_t) -> hv_return_t

Sets the generic interrupt controller (GIC) distributor region’s base address.

func hv_gic_config_set_redistributor_base(hv_gic_config_t, hv_ipa_t) -> hv_return_t

Sets the generic interrupt controller (GIC) redistributor region base address.

func hv_gic_get_redistributor_base(hv_vcpu_t, UnsafeMutablePointer&lt;hv_ipa_t>) -> hv_return_t

Gets the redistributor base guest physical address for the given vCPU.

func hv_gic_config_set_msi_interrupt_range(hv_gic_config_t, UInt32, UInt32) -> hv_return_t

Sets the range of message signaled interrupts (MSIs) the generic interrupt controller supports.

protocol OS_hv_gic_config

Methods that provide information on the state of a generic interrupt controller.

typealias hv_gic_config_t

An alias for this value type’s equivalent Hypervisor generic interrupt controller (GIC) configuration’s reference type.

