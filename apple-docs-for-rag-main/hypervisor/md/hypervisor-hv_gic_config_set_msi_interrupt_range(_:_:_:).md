

- Hypervisor
-  hv_gic_config_set_msi_interrupt_range(\_:\_:\_:) 

Function

# hv_gic_config_set_msi_interrupt_range(\_:\_:\_:)

Sets the range of message signaled interrupts (MSIs) the generic interrupt controller supports.

macOS 15.0+

``` source
func hv_gic_config_set_msi_interrupt_range(
    _ config: hv_gic_config_t,
    _ msi_intid_base: UInt32,
    _ msi_intid_count: UInt32
) -> hv_return_t
```

## Parameters 

`config`  

A generic interrupt controller (GIC) configuration object.

`msi_intid_base`  

The lowest MSI interrupt number.

`msi_intid_count`  

Number of message signaled interrupts.

## Return Value

HV_SUCCESS on success; otherwise, an error code.

## Discussion

Use this method to configure the range of identifiers supported for MSIs. If it’s outside of the range given by hv_gic_get_spi_interrupt_range(_:_:), the method returns an error.

Set the region base address with hv_gic_config_set_msi_region_base(_:_:).

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

func hv_gic_config_set_msi_region_base(hv_gic_config_t, hv_ipa_t) -> hv_return_t

Sets the generic interrupt controllers message signaled interrupts (MSIs) region base address.

protocol OS_hv_gic_config

Methods that provide information on the state of a generic interrupt controller.

typealias hv_gic_config_t

An alias for this value type’s equivalent Hypervisor generic interrupt controller (GIC) configuration’s reference type.

