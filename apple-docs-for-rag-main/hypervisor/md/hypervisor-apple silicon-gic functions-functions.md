

- Hypervisor
- Apple Silicon
-  GIC functions 

API Collection

# GIC functions

These functions and registers support the creation and operation of a generic interrupt controller.

## Discussion

For more information on using GICs, see the ARM Generic Interrupt Controller (GIC) v3 architecture specification.

## Topics

### Creating a generic interrupt controller

func hv_gic_create(hv_gic_config_t) -> hv_return_t

Creates a generic interrupt controller (GIC) v3 device for a VM configuration.

### Resetting the generic interrupt controller

func hv_gic_reset() -> hv_return_t

Resets the generic interrupt controller (GIC) device.

### Setting the GIC device configuration

Setting the configuration of a generic interrupt controller involves configuring the memory addresses for the various GIC subcomponents. Use these methods to set the interrupt distributor and redistributor base addresses, and set up the interrupt range for the message signaled interrupts (MSIs).

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

typealias hv_gic_config_t

An alias for this value type’s equivalent Hypervisor generic interrupt controller (GIC) configuration’s reference type.

### Getting GIC device parameters

func hv_gic_get_redistributor_region_size(UnsafeMutablePointer&lt;Int>) -> hv_return_t

Gets the total size in bytes of the generic interrupt controller (GIC) redistributor region.

func hv_gic_get_redistributor_size(UnsafeMutablePointer&lt;Int>) -> hv_return_t

Gets the size in bytes of a single generic interrupt controller (GIC) redistributor.

func hv_gic_get_distributor_size(UnsafeMutablePointer&lt;Int>) -> hv_return_t

Gets the size of the generic interrupt controller (GIC) distributor region, in bytes.

func hv_gic_get_distributor_base_alignment(UnsafeMutablePointer&lt;Int>) -> hv_return_t

Gets the alignment for the base address of the generic interrupt controller (GIC) distributor region, in bytes.

func hv_gic_get_redistributor_base_alignment(UnsafeMutablePointer&lt;Int>) -> hv_return_t

Gets the alignment for the base address of the generic interrupt controller (GIC) redistributor region, in bytes.

func hv_gic_get_msi_region_base_alignment(UnsafeMutablePointer&lt;Int>) -> hv_return_t

Gets the alignment, in bytes, for the base address of the generic interrupt controller’s message signaled interrupts (MSI) region.

func hv_gic_get_msi_region_size(UnsafeMutablePointer&lt;Int>) -> hv_return_t

Gets the size in bytes of the generic interrupt controller’s (GIC) message signaled interrupts (MSI) region.

func hv_gic_get_spi_interrupt_range(UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;UInt32>) -> hv_return_t

Gets the range of shared peripheral interrupts (SPIs) the generic interrupt controller supports.

### Getting and setting the GIC’s state

These methods manage the register values in the generic interrupt controller (GIC) hardware and metadata associated with them. Use them to save and restore the state of the GIC.

func hv_gic_state_create() -> hv_gic_state_t

Create a generic interrupt controller (GIC) state object.

func hv_gic_set_state(UnsafeRawPointer, Int) -> hv_return_t

Sets the state of a generic interrupt controller (GIC) device.

func hv_gic_state_get_size(hv_gic_state_t, UnsafeMutablePointer&lt;Int>) -> hv_return_t

Gets the size of the buffer required for generic interrupt controller (GIC) state.

func hv_gic_state_get_data(hv_gic_state_t, UnsafeMutableRawPointer) -> hv_return_t

Gets the state data for generic interrupt controller (GIC).

typealias hv_gic_state_t

An alias for this value type’s equivalent Hypervisor generic interrupt controller (GIC) state’s reference type.

protocol OS_hv_gic_state

Methods that provide information on the hypervisor state.

### Sending interrupts

func hv_gic_send_msi(hv_ipa_t, UInt32) -> hv_return_t

Sends a message signaled interrupt (MSI).

func hv_gic_set_spi(UInt32, Bool) -> hv_return_t

Triggers a shared peripheral interrupt (SPI).

### Getting and setting registers

func hv_gic_get_distributor_reg(hv_gic_distributor_reg_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Reads a generic interrupt controller (GIC) distributor register.

func hv_gic_get_msi_reg(hv_gic_msi_reg_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Reads a generic interrupt controller (GIC) distributor message signaled interrupt (MSI) register.

func hv_gic_get_icc_reg(hv_vcpu_t, hv_gic_icc_reg_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Reads a generic interrupt controller’s ICC CPU system register.

func hv_gic_get_ich_reg(hv_vcpu_t, hv_gic_ich_reg_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Reads a generic interrupt controller’s (GIC) ICH virtualization control system register.

func hv_gic_get_icv_reg(hv_vcpu_t, hv_gic_icv_reg_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Writes a generic interrupt controller’s (GIC) ICV system register.

func hv_gic_get_redistributor_reg(hv_vcpu_t, hv_gic_redistributor_reg_t, UnsafeMutablePointer&lt;UInt64>) -> hv_return_t

Read a generic interrupt controller (GIC) redistributor register.

func hv_gic_set_distributor_reg(hv_gic_distributor_reg_t, UInt64) -> hv_return_t

Writes the provided value to a generic interrupt controller (GIC) distributor register you specify.

func hv_gic_set_icc_reg(hv_vcpu_t, hv_gic_icc_reg_t, UInt64) -> hv_return_t

Writes to a generic interrupt controller (GIC) ICC cpu system register.

func hv_gic_set_ich_reg(hv_vcpu_t, hv_gic_ich_reg_t, UInt64) -> hv_return_t

Writes to a generic interrupt controller (GIC) ICH virtualization control system register.

func hv_gic_set_icv_reg(hv_vcpu_t, hv_gic_icv_reg_t, UInt64) -> hv_return_t

Writes to a generic interrupt controller (GIC) ICV system register.

func hv_gic_set_msi_reg(hv_gic_msi_reg_t, UInt64) -> hv_return_t

Writes to a generic interrupt controller distributor message signaled interrupt (MSI) register.

func hv_gic_set_redistributor_reg(hv_vcpu_t, hv_gic_redistributor_reg_t, UInt64) -> hv_return_t

Writes to a GIC redistributor register.

## See Also

### Generic interrupt controllers (GICs)

GIC registers

These registers support the operation of a generic interrupt controller and its interface with the Hypervisor and virtual CPUs.

