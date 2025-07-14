

- Hypervisor
-  hv_gic_config_t 

Type Alias

# hv_gic_config_t

An alias for this value type’s equivalent Hypervisor generic interrupt controller (GIC) configuration’s reference type.

macOS

``` source
typealias hv_gic_config_t = any OS_hv_gic_config
```

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

func hv_gic_config_set_msi_interrupt_range(hv_gic_config_t, UInt32, UInt32) -> hv_return_t

Sets the range of message signaled interrupts (MSIs) the generic interrupt controller supports.

protocol OS_hv_gic_config

Methods that provide information on the state of a generic interrupt controller.

