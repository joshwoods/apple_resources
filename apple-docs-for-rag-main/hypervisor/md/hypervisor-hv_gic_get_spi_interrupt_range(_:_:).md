

- Hypervisor
-  hv_gic_get_spi_interrupt_range(\_:\_:) 

Function

# hv_gic_get_spi_interrupt_range(\_:\_:)

Gets the range of shared peripheral interrupts (SPIs) the generic interrupt controller supports.

macOS 15.0+

``` source
func hv_gic_get_spi_interrupt_range(
    _ spi_intid_base: UnsafeMutablePointer,
    _ spi_intid_count: UnsafeMutablePointer
) -> hv_return_t
```

## Parameters 

`spi_intid_base`  

A pointer to the lowest SPI number that the framework writes to upon success.

`spi_intid_count`  

A pointer to the number of SPIs supported that the framework writes to upon success.

## Return Value

HV_SUCCESS on success; otherwise, an error code.

## See Also

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

