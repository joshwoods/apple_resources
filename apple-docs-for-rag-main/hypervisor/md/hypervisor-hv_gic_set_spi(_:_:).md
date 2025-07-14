

- Hypervisor
-  hv_gic_set_spi(\_:\_:) 

Function

# hv_gic_set_spi(\_:\_:)

Triggers a shared peripheral interrupt (SPI).

macOS 15.0+

``` source
func hv_gic_set_spi(
    _ intid: UInt32,
    _ level: Bool
) -> hv_return_t
```

## Parameters 

`intid`  

The interrupt number of the SPI.

`level`  

The high- or low-level state for the interrupt. Setting the level also causes an edge on the line for an edge triggered interrupt.

## Return Value

HV_SUCCESS on success; otherwise, an error code.

## Discussion

Setting a level value causes level interrupts. To cause an edge interrupt, call this method with a level of true. The framework ignores a level of false for an edge interrupt.

An interrupt identifier outside of hv_gic_get_spi_interrupt_range(_:_:) or in the message signaled interrupt (MSI) range returns a HV_BAD_ARGUMENT error code.

## See Also

### Sending interrupts

func hv_gic_send_msi(hv_ipa_t, UInt32) -> hv_return_t

Sends a message signaled interrupt (MSI).

