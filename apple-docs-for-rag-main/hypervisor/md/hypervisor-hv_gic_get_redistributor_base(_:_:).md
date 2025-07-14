

- Hypervisor
-  hv_gic_get_redistributor_base(\_:\_:) 

Function

# hv_gic_get_redistributor_base(\_:\_:)

Gets the redistributor base guest physical address for the given vCPU.

macOS 15.0+

``` source
func hv_gic_get_redistributor_base(
    _ vcpu: hv_vcpu_t,
    _ redistributor_base_address: UnsafeMutablePointer
) -> hv_return_t
```

## Parameters 

`vcpu`  

Handle for the vCPU.

`redistributor_base_address`  

A pointer to the redistributor base guest physical address that the framework writes to upon success.

## Return Value

HV_SUCCESS on success; otherwise, an error code.

## Discussion

Important

Call this method after you set the affinity of the given vCPU in its `MPIDR_EL1` register.

## See Also

### Setting the GIC device configuration

func hv_gic_config_create() -> hv_gic_config_t

Creates a generic interrupt controller (GIC) configuration object.

func hv_gic_config_set_distributor_base(hv_gic_config_t, hv_ipa_t) -> hv_return_t

Sets the generic interrupt controller (GIC) distributor region’s base address.

func hv_gic_config_set_redistributor_base(hv_gic_config_t, hv_ipa_t) -> hv_return_t

Sets the generic interrupt controller (GIC) redistributor region base address.

func hv_gic_config_set_msi_region_base(hv_gic_config_t, hv_ipa_t) -> hv_return_t

Sets the generic interrupt controllers message signaled interrupts (MSIs) region base address.

func hv_gic_config_set_msi_interrupt_range(hv_gic_config_t, UInt32, UInt32) -> hv_return_t

Sets the range of message signaled interrupts (MSIs) the generic interrupt controller supports.

protocol OS_hv_gic_config

Methods that provide information on the state of a generic interrupt controller.

typealias hv_gic_config_t

An alias for this value type’s equivalent Hypervisor generic interrupt controller (GIC) configuration’s reference type.

